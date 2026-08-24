# Interface architecture

The initial architecture translates the priority workflows into a consistent operational workspace. The full design inventory plans 84 surfaces; this document summarizes the public information architecture rather than reproducing the internal screen specification.

## Global shell

- stable modules in a vertical sidebar;
- clinic and unit context visible throughout the application;
- global search, tasks, notifications and user preferences;
- breadcrumbs and contextual actions where hierarchy matters;
- navigation filtered by effective permissions.

## Main work areas

1. Dashboard and operational priorities
2. Schedule and resource availability
3. Patients and patient workspace
4. Clinical care and documentation
5. Pilates classes and participants
6. Packages, contracts and credits
7. Finance and closing
8. Documents and communication
9. Reports and clinic settings
10. Personal settings and platform back office

CRM capabilities remain outside the first release and do not reuse the patient record as a sales lead.

## Patient workspace

A persistent patient header anchors administrative, scheduling, package, financial and clinical views. Tabs and actions are filtered by permission so restricted content is not partially revealed.

## Interaction surfaces

- drawers for quick, contextual tasks such as registration, scheduling and payments;
- dedicated pages for complex clinical or configuration work;
- dialogs for risk, scope and impact decisions;
- tables for dense operational comparison and lists/cards on smaller screens;
- persistent notices for blocking issues and transient feedback for completed actions.

## Responsive direction

Mobile is treated as a task-focused layout, not a scaled-down desktop. Navigation, filters, forms and data lists may change structure while preserving the same permissions and workflow meaning.

## Architecture constraints

- new requirements should prefer contextual states before adding primary screens;
- finalized records remain immutable and corrections are explicit;
- tenant, clinic and unit context must never be ambiguous;
- status, errors, loading and empty states are part of every surface;
- charts require a meaningful comparison and an accessible alternative.

## Contextual registration update

The appointment editor and quick patient registration now form a subflow. Registration opens over the schedule, preserves the appointment draft and returns the newly created patient to the selector. This change uses existing surfaces rather than adding a new route to the architecture.

## Collective Pilates update

The schedule editor switches between single-patient selection and multi-participant selection based on the service. Schedule cards summarize class and occupancy, while class detail exposes a participant roster and contextual bulk addition. Capacity, waiting-list and individual participant states are expressed through existing schedule and Pilates surfaces.
