# Prototype evolution

This document records verified prototype milestones without claiming that simulated behavior is production-ready.

The prototype began as FisioFlow and later adopted the official Movune name. Earlier sections intentionally preserve the name visible at each stage.

## First navigable FisioFlow slice

The initial prototype introduced a shared shell and four navigable areas:

- Dashboard;
- Schedule;
- Patients;
- Patient profile.

It used fictional clinic and patient data to explore navigation, cards, a weekly schedule, patient lists and contextual detail. The first visual language had a dark shell with a strong green presence, a vertical sidebar, a separate top bar and rounded content surfaces.

## Early consistency pass

The first review grouped small visual issues instead of treating each as a product milestone. It improved compact-sidebar behavior, avatar alignment, card actions, badges and the schedule's visual layering. Events were separated from grid lines and positioned by time and duration.

## Limits at this stage

The prototype was a front-end demonstration. It did not prove backend persistence, real integrations, a complete permissions engine or implementation of all planned surfaces. Pilates could appear in the schedule, but the collective attendance model had not yet been demonstrated.

## Contextual registration in scheduling

The appointment editor gained an action to create a patient without abandoning the form. The prototype demonstrated preserved appointment data, duplicate and recoverable-error states, automatic selection after creation and distinct feedback for each saved object.

## Collective Pilates occurrence

The prototype replaced the single-patient assumption for Pilates with one class occurrence containing multiple participants. Schedule cards show occupancy, class details expose an individual roster, and participant addition demonstrates capacity, duplicate prevention and waiting-list states. The prototype still uses fictional fixed scenarios rather than a complete scheduling engine.

## Semantic action feedback

The prototype introduced consistent success, error, warning and information messages with titles, descriptions, dismiss actions and recoverable next steps. Simulated WhatsApp and calendar operations distinguish a local save from external processing and failure.

## Deterministic scheduling states

Conflict scenarios now identify professional, room or equipment and preserve the form while offering alternatives. Cancelled events disappear from the operational grid but remain visible in the fictional patient's timeline. Pilates cancellation releases an individual place without removing the collective occurrence.

## Finite recurrence preview

The schedule editor gained non-recurring and recurring modes, weekday-specific times and a preview of date range, totals, capacity, conflicts and plan eligibility. Fixed fictional scenarios demonstrate validation and scope decisions; they do not represent a production recurrence engine.

## Rename to Movune

The product name changed from FisioFlow to Movune after the core scheduling and Pilates rules had been consolidated. The rename did not alter the approved product scope, 23 priority flows or planned interface inventory. Visual identity changes followed as a distinct design step.

## First Movune identity application

The prototype adopted the Movune name, circular M concept, teal palette and updated typography across the shared shell, Dashboard, Schedule, Patients and Patient profile. The Dashboard shifted toward today's operation, and schedule cards separated service from appointment status. The first application exposed new visual issues that were refined afterward.
