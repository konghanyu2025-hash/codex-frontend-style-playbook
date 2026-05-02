# Implementation Brief

## Scope

Build a single-page portfolio site for an independent interaction designer.

## Layout

Use a first viewport that presents the designer's name, role, positioning, primary contact action, and a visible hint of selected work. Follow with case studies, process, credibility, and contact.

## Navigation

Top navigation includes Work, Process, About, and Contact. Keep it compact and readable.

## Components

- First-viewport identity block.
- Featured project previews.
- Process snapshots.
- Credibility row.
- Contact block.

## Typography

Use editorial hierarchy, but keep all text within containers. Avoid viewport-width font scaling. Use smaller headings inside compact sections.

## Color

Use a neutral base and one strong accent. Avoid one-note palettes and generic gradient backgrounds.

## Imagery and Media

Use project-relevant interface imagery or generated placeholder visuals that look like real product work. Avoid purely atmospheric stock-style visuals.

## Interactions and States

Project previews can have subtle hover states. Contact links need clear focus states.

## Responsive Behavior

- Desktop: first viewport can use an editorial composition with visible next-section hint.
- Mobile: stack name, role, contact, and first work preview without clipping.
- Project previews keep fixed aspect ratios.

## Accessibility

Maintain text contrast. Links and buttons require visible focus. Images need useful alt text.

## QA Criteria

- Name and role are visible in the first viewport.
- At least one work preview is visible or hinted before the fold.
- Mobile has no clipped display type.
- Visual assets reveal work, not just atmosphere.
