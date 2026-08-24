# Movune design principles

These principles began during the FisioFlow exploration and continue under the official Movune name. The UI/UX direction aims for an operational SaaS that is calm, legible and efficient without looking clinical or bureaucratic.

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

## Movune identity layer

Movune adds a movement-and-connection brand concept, a teal institutional palette, Manrope headings and Inter interface text. Institutional color remains separate from semantic state and service colors. Schedule items therefore communicate appointment status and service type through independent visual and textual channels.

The desktop shell uses a compact, recognizable sidebar and a minimal top bar. Mobile receives a dedicated priority navigation rather than a compressed desktop sidebar.

## Current shell behavior

- desktop sidebar is compact by default and expands on hover;
- the Movune symbol remains visible in compact mode;
- the top bar is visually integrated with the content through a restrained divider;
- dark mode uses neutral graphite surfaces with teal reserved for brand and active states;
- global and contextual add actions share the same brand token;
- major overlays close by outside click or `Esc` when it is safe to do so.

Appearance preferences use visual choices for light, dark or system theme and text scales of 100%, 114% and 128%. A previously explored density preference was removed from the current prototype to reduce unnecessary complexity.

## Semantic feedback

Actions use four explicit feedback meanings: success, error, warning and information. Each message combines text and iconography instead of relying on color alone.

- transient feedback confirms immediate local results;
- blocking validation remains visible beside the affected context;
- recoverable failures offer a safe next action;
- external operations begin as requested or processing and only report completion after confirmation;
- persistent integration failures remain discoverable in notifications or tasks.

Feedback never includes clinical or financial detail that the current viewer is not authorized to see.
