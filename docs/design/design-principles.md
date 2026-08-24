# Initial design principles

FisioFlow's first UI/UX direction aims for an operational SaaS that is calm, legible and efficient without looking clinical or bureaucratic.

## Experience principles

- keep the next action in context;
- prefer recognition over memorization;
- make priorities and pending work clearer than passive metrics;
- confirm actions in proportion to their risk;
- preserve entered data when validation or an integration fails;
- hide unauthorized content instead of exposing disabled details;
- separate current state from historical evidence.

## Visual direction

- neutral backgrounds with restrained elevation;
- rounded cards, controls and overlays;
- denser schedules and tables, with more breathing room in clinical forms;
- consistent hierarchy across headings, labels, supporting text and status;
- charts only when they improve comparison or trend reading.

The visual references used during exploration informed patterns such as the sidebar, dashboard cards, tables and schedule grid. They are not product assets and are not published in this repository.

## Interaction patterns

- a collapsible sidebar for stable desktop navigation;
- contextual drawers for quick tasks;
- explicit validation before drag-and-drop changes become final;
- visible loading, empty, success, warning and error states;
- keyboard access, focus visibility and semantic labels;
- light, dark and system themes with adjustable text size.

## Responsive behavior

Desktop prioritizes dense daily operation. Tablet and mobile reorganize navigation, filters and tables around the most frequent tasks instead of shrinking the desktop layout.

## Accessibility baseline

The direction targets WCAG 2.2 AA contrast, keyboard navigation, screen-reader semantics, reduced motion support, touch-friendly targets and text enlargement without loss of content or function.

## Semantic feedback

Actions use four explicit feedback meanings: success, error, warning and information. Each message combines text and iconography instead of relying on color alone.

- transient feedback confirms immediate local results;
- blocking validation remains visible beside the affected context;
- recoverable failures offer a safe next action;
- external operations begin as requested or processing and only report completion after confirmation;
- persistent integration failures remain discoverable in notifications or tasks.

Feedback never includes clinical or financial detail that the current viewer is not authorized to see.
