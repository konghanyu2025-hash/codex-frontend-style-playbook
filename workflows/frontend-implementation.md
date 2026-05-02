# Frontend Implementation Workflow

Use this workflow after `style_brief.md` and `visual_anchor.md` are complete.

## Goal

Turn the visual direction into a real frontend that works in the target project.

## Implementation Brief

Before coding, create `implementation_brief.md`:

```md
# Implementation Brief

## Scope

## Layout

## Navigation

## Components

## Typography

## Color

## Imagery and Media

## Interactions and States

## Responsive Behavior

## Accessibility

## QA Criteria
```

## Build Rules

- Use the existing project stack and conventions.
- Start with structure and content hierarchy before decorative styling.
- Build complete states for repeated interactive elements.
- Prefer semantic HTML where possible.
- Use icons only when they clarify a known action.
- Keep cards, panels, and controls stable across hover, loading, and selected states.
- Make responsive behavior explicit for desktop, tablet, and mobile.
- Use real content or realistic placeholders that match the product.

## Layout Rules

- Define max widths, grid tracks, aspect ratios, and stable toolbar dimensions.
- Do not rely on viewport-width font scaling.
- Do not let content changes resize navigation or control surfaces unexpectedly.
- Avoid nested cards unless the nested surface is truly a modal, repeated item, or framed tool.
- Avoid large decorative sections when the product is an operational tool.

## Visual Rules

- Convert the anchor into tokens: background, surface, text, accent, border, muted text, danger, success, and focus.
- Use a clear type scale with limited heading levels.
- Keep letter spacing at normal unless the design system already uses a specific setting.
- Check that contrast is sufficient for important text and controls.
- Do not let the palette collapse into many variations of one hue unless the brief requires it.

## Done Criteria

Implementation is done only when:

- The UI runs locally.
- Desktop and mobile screenshots have been reviewed.
- The result matches `implementation_brief.md`.
- The primary workflow is visible and usable.
- The result looks intentionally designed, not merely styled.
