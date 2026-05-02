# Visual Anchor

## Inputs

This example assumes Codex generated three GPT Image 2 visual anchors:

1. Dense executive dashboard with left navigation and compact KPI grid.
2. Forecast command center with risk queue and activity rail.
3. Operational table-first dashboard with charts as supporting context.

## Anchor Images

Images are not committed in this example. In a real task, store generated images or screenshots in the project artifact area and reference their paths here.

## Keep

- Compact left navigation.
- Top filter bar with team, quarter, segment, and date controls.
- KPI row that shows current value, change, and confidence.
- Risk queue placed near the top-right for repeated daily use.
- Muted surfaces with strong text contrast.
- Small but readable charts with labels.

## Reject

- Full-screen decorative background.
- Huge hero header.
- Overly rounded glass cards.
- Chart-only dashboard with no action surface.
- Tiny fake labels that cannot become real UI.

## Design Tokens to Extract

- Background: neutral off-white or very light cool gray.
- Surface: white or near-white.
- Border: low-contrast neutral.
- Text: high-contrast neutral.
- Muted text: mid-gray.
- Accent: one clear action color.
- Risk: warm red or amber, used sparingly.

## Layout Rules

- Use a persistent left navigation on desktop.
- Use a compact top filter row.
- Use a 12-column dashboard grid.
- Keep the risk queue visible in the first viewport.
- Keep table rows dense but readable.

## Component Rules

- KPI cards need value, label, trend, and context.
- Risk items need severity, owner, account, and recommended action.
- Tables need clear status pills and sortable columns.
- Charts should have legends and direct labels where possible.

## Responsive Implications

- Mobile should collapse navigation into a top bar or drawer.
- KPI cards become a two-column grid, then one column below narrow widths.
- Tables need horizontal handling or a card representation.

## Implementation Risks

- Too much gray can feel unfinished.
- Too many accent colors can weaken severity signals.
- Tables can overflow mobile if columns are not prioritized.
