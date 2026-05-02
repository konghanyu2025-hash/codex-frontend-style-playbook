# Implementation Brief

## Scope

Build one dashboard screen for a B2B revenue operations product.

## Layout

Use a desktop layout with left navigation, top filter bar, KPI strip, chart and risk panels, and a dense opportunity table. Mobile collapses into a single-column workflow with navigation hidden behind a menu.

## Navigation

Left nav includes Dashboard, Forecast, Accounts, Deals, Activity, and Settings. The active item is Dashboard.

## Components

- KPI cards.
- Forecast chart panel.
- Risk queue.
- Deal movement timeline.
- Opportunity table.
- Filter controls.
- Status pills.

## Typography

Use a restrained type scale. Dashboard titles should be smaller than marketing hero text. Metric values can be prominent but must not dominate the screen.

## Color

Use neutral backgrounds and surfaces. Reserve accent color for primary actions and selected states. Reserve red or amber for risk.

## Imagery and Media

No decorative imagery is needed. Use charts and data views as the primary visual content.

## Interactions and States

Include hover, selected, focus, empty, loading, and risk severity states where relevant.

## Responsive Behavior

- Desktop: full dashboard grid.
- Tablet: navigation compresses, grid becomes two columns.
- Mobile: sections stack by priority, filters become compact controls, table becomes cards or prioritized rows.

## Accessibility

All controls need accessible names. Risk color must be paired with text or icon labels. Focus states must be visible.

## QA Criteria

- No horizontal scroll on mobile unless the table intentionally uses a scroll container.
- Risk queue is visible in the first desktop viewport.
- KPI labels do not wrap awkwardly.
- Primary action is visible.
- Charts are readable and not decorative filler.
