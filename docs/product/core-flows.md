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
