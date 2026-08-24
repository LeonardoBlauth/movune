# Movune product overview

## Problem

Small and medium-sized physiotherapy and Pilates clinics often combine paper records, spreadsheets, generic calendars and disconnected systems. The result is repeated data entry, scheduling conflicts, weak operational visibility and fragmented follow-up across care, classes, packages and payments.

## Product direction

Movune is a B2B SaaS designed to keep the clinic's daily operation in one workspace. The project was initially known as FisioFlow. A person has a single administrative identity inside a clinic and can participate in physiotherapy and Pilates journeys without duplicating their history.

The initial product direction assumes:

- isolated clinic accounts in a multi-tenant platform;
- support for multiple units, professionals and users;
- role- and scope-based permissions;
- explicit separation of clinical, administrative and financial information;
- traceable changes for sensitive records;
- accessible light and dark themes with adjustable text size.

## Initial scope

The first sellable release is expected to cover:

- dashboard and operational tasks;
- scheduling and resource availability;
- patients and clinical records;
- assessments, treatment plans and progress notes;
- Pilates classes and attendance;
- packages, contracts and session credits;
- receivables and basic financial operations;
- documents, transactional communication and notifications;
- users, permissions, clinic settings and personal preferences.

Advanced CRM, deeper automation, intelligence features and broader integrations remain later-stage opportunities. They must not complicate the core clinic workflow.

## Product principles

1. Keep the next action close to the current context.
2. Preserve auditability instead of silently overwriting finalized facts.
3. Treat attendance, clinical documentation, credit consumption and payment as separate events.
4. Make permissions visible in both data access and interface actions.
5. Prefer supervised automation with recoverable failures.

## Current stage

The product is in definition and prototyping. This document records product intent, not proof of a production implementation.

## Collective Pilates model

Pilates is modeled as a collective occurrence for a class and time interval rather than a collection of unrelated individual appointments. Capacity belongs to the applicable class and resources, while reservation, contract, confirmation, attendance and credit consumption remain individual for every participant.

## Finite recurring schedules

Recurring schedules are bounded by treatment or participation plans. A series can use several weekdays with a different time on each day. It is previewed before creation and never produces an open-ended sequence.
