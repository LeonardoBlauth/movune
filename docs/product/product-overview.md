# Movune product overview

## Origin

Movune started from a real operational need observed in a small physiotherapy and Pilates clinic that struggled to adapt its workflow to the management software it had tried.

The initial context is intentionally simple: a single clinic operated by a single professional, combining physiotherapy and Pilates activities.

The project began by exploring how software could better support that operation. As requirements, workflows and interface decisions were developed, the scope expanded to consider more complex clinic structures and operational needs.

## Product direction

Movune explores a clinic management platform that brings scheduling, patient administration, clinical workflows, Pilates operations, packages, finance and communication into a connected workspace. A person has a single administrative identity inside a clinic and can participate in physiotherapy and Pilates journeys without duplicating their history.

The current direction considers scenarios beyond the initial clinic, including:

- isolated clinic accounts in a multi-tenant platform;
- support for multiple units, professionals and users;
- role- and scope-based permissions;
- explicit separation of clinical, administrative and financial information;
- traceable changes for sensitive records;
- accessible light and dark themes with adjustable text size.

These scenarios represent the current product direction and may evolve as the initial workflows are prototyped, tested and refined.

## Initial scope

The current scope includes:

- dashboard and operational tasks;
- scheduling and resource availability;
- patients and clinical records;
- assessments, treatment plans and progress notes;
- Pilates classes and attendance;
- packages, contracts and session credits;
- receivables and basic financial operations;
- documents, transactional communication and notifications;
- users, permissions, clinic settings and personal preferences.

Advanced CRM, deeper automation, intelligence features and broader integrations remain possible later-stage directions and should not complicate the core clinic workflow.

## Product principles

1. Keep the next action close to the current context.
2. Preserve auditability instead of silently overwriting finalized facts.
3. Treat attendance, clinical documentation, credit consumption and payment as separate events.
4. Make permissions visible in both data access and interface actions.
5. Prefer supervised automation with recoverable failures.

## Current stage

Movune is currently in product definition and prototyping.

The current documentation describes intended product behavior and decisions being explored. It should not be interpreted as proof of a production implementation.

The prototype is being used to refine the initial workflows before defining the MVP and technical architecture.

## Collective Pilates model

Pilates is modeled as a collective occurrence for a class and time interval rather than a collection of unrelated individual appointments. Capacity belongs to the applicable class and resources, while reservation, contract, confirmation, attendance and credit consumption remain individual for every participant.

## Finite recurring schedules

Recurring schedules are bounded by treatment or participation plans. A series can use several weekdays with a different time on each day. It is previewed before creation and never produces an open-ended sequence.
