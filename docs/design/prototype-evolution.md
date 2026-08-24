# Prototype evolution

This document records verified prototype milestones without claiming that simulated behavior is production-ready.

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
