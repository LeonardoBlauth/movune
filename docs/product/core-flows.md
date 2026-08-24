# Core product flows

FisioFlow's initial workflow map covers the clinic lifecycle from account setup to daily operation and reporting. The internal specification contains 23 priority flows; this public summary groups them without exposing implementation-level detail.

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
