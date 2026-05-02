# Visual Anchor

## Inputs

This example assumes Codex generated three GPT Image 2 visual anchors:

1. Typography-led portfolio with structured case study strips.
2. Full-bleed editorial first viewport with project thumbnails visible below.
3. Dense interaction-design portfolio with annotated interface fragments.

## Anchor Images

Images are not committed in this example. In a real task, store generated images or screenshots in the project artifact area and reference their paths here.

## Keep

- Name and role as the strongest first-viewport signal.
- Immediate proof of complex interface work.
- Project previews that reveal actual interface details.
- Editorial typography with clear hierarchy.
- Restrained accent system.

## Reject

- Abstract-only hero art.
- Empty first viewport.
- Project cards that hide all work context.
- Decorative motion that delays reading.
- Generic beige or purple portfolio palette unless requested.

## Design Tokens to Extract

- Background: neutral base with one distinctive contrast surface.
- Surface: minimal, mostly unframed.
- Text: high-contrast editorial scale.
- Accent: one vivid but controlled color.
- Borders: used for structure, not decoration.

## Layout Rules

- First viewport must show name, role, positioning, primary contact action, and a preview of selected work.
- Case studies should appear as wide rows or editorial blocks, not generic cards inside cards.
- Keep content bands full-width with constrained inner content.

## Component Rules

- Project previews need title, domain, role, outcome, and image or interface evidence.
- Contact action must be obvious.
- Navigation can be compact but must be visible.

## Responsive Implications

- Mobile should lead with name, role, and first work preview.
- Project media should maintain aspect ratio.
- Long project titles must wrap cleanly.

## Implementation Risks

- Editorial type can become too large for mobile.
- Decorative layout can hide the work.
- Strong accent colors can overpower project content.
