# Core product flows

Movune's workflow map covers the clinic lifecycle from account setup to daily operation and reporting. The internal specification contains 23 priority flows; this public summary groups them without exposing implementation-level detail.

## Clinic setup and access

- create a clinic and its first unit;
- invite users and professionals with scoped permissions;
- configure services, resources, rooms and operational policies;
- keep platform administration separate from clinic navigation.

## Patient and care journey

- register a person once and progressively complete required data;
- start or update a care episode through an assessment;
- create a versioned treatment plan;
- record progress as a draft, finalize it explicitly and correct it through an addendum;
- keep clinical detail hidden from roles that only need operational facts.

## Scheduling

- find availability by professional, service, unit and resource;
- create, reschedule or cancel an appointment with an explicit status;
- distinguish individual appointments from class-based activities;
- preserve history and audit information for operational changes.

## Pilates operations

- configure recurring class models, capacity and resources;
- enroll participants and manage attendance;
- keep each participant's contract, presence and credit movement independent;
- support a waiting list when capacity is reached.

## Packages and finance

- sell a versioned offer and activate it under the configured policy;
- derive balances from credit movements instead of an editable counter;
- record receivables, payments, reversals and closing activities;
- avoid coupling payment status to clinical record completion.

## Communication and automation

- send transactional messages from an authorized context;
- synchronize eligible events with external calendars;
- expose processing, failure and retry states for external operations;
- keep sensitive automation traceable and pausable.

## Flow invariants

Every flow must preserve tenant isolation, permissions, auditability and recoverable failure states. This is a product blueprint; integrations and business engines are not yet implemented.

## Contextual patient registration

Scheduling now supports a lightweight registration subflow when a search does not find the patient:

1. keep the appointment form and its current values;
2. open the minimum patient registration in context;
3. check likely duplicates before creating a record;
4. return to scheduling with the new patient selected;
5. report patient creation and appointment creation as separate outcomes.

The regular Patients area remains available for standalone registration. The contextual flow reduces navigation without weakening identity checks.

## Collective Pilates scheduling

An individual care appointment continues to select one patient. A Pilates class uses one collective occurrence with multiple participant reservations.

- the participant list respects class and resource capacity;
- the same person cannot be added twice;
- each participant keeps independent contract, confirmation, attendance and credit state;
- a full occurrence can offer a waiting-list path;
- adding or cancelling one participant changes only that reservation;
- selecting the same class and interval reuses the existing occurrence instead of creating a duplicate.

## Feedback across flows

Create, edit, removal, configuration and integration requests return a semantic result in the action context. An external failure does not silently undo a successful local save; it creates a visible pending state and a retry path when safe. Messages distinguish the saved domain object from follow-up processing such as messaging or calendar synchronization.

## Scheduling availability and cancellation

Active appointments cannot overlap when they reserve the same professional, room or equipment. This is a hard availability rule; permission does not bypass a real competing reservation. Parallel care remains possible when resources are distinct.

The scheduling flow identifies the conflicting resource and can suggest a different time or room while preserving the draft. If the occupied slot is the same Pilates class, the user is directed to add participants to that occurrence subject to capacity.

Cancellation and late cancellation immediately release the reserved slot and resources. Cancelled records leave the operational grid but remain in patient history and audit records with status and reason. Financial or credit consequences continue to follow the applicable policy and are not inferred from grid visibility.

## Plan-based recurrence

Scheduling offers a single occurrence or a finite weekly series. A recurring series requires a plan with an end date and supports multiple weekdays with an independent time for each day.

Before creation, the user reviews the first and last dates, occurrence count, resource conflicts, capacity and participant eligibility. For a collective occurrence, the series can extend to the latest participant plan end date, but each occurrence includes only participants eligible on that date. Empty occurrences are not created.

Editing or cancelling a member of a series requires an explicit scope: only this occurrence, this and future occurrences, or the entire series. The selected scope is revalidated against resources, capacity, plans and contracts.
