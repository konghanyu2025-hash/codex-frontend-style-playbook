# Frontend Agent Rules

These rules apply when an agent uses this repository to build or improve a frontend.

## Goal

Build a real, usable frontend whose style is grounded in references and visual anchors, then verified through screenshots.

Do not rely on vague taste words. Convert them into layout, density, typography, color, component, motion, and responsive rules before implementation.

## Required Process

1. Read the task and identify the product category, user, primary workflow, and required content.
2. Follow `workflows/style-discovery.md`.
3. Follow `workflows/gpt-image-2-anchor.md`.
4. Produce `style_brief.md`, `visual_anchor.md`, and `implementation_brief.md`.
5. Implement only after those briefs are specific enough to build from.
6. Follow `workflows/visual-qa.md` before final delivery.

## Frontend Standards

- Build the actual product screen, app, tool, or site. Do not default to a marketing landing page unless the user asked for one.
- Prefer the existing project stack, component system, CSS conventions, icons, routing, and data patterns.
- Use realistic information architecture and user flows.
- Make the first screen useful, not just decorative.
- Use stable dimensions for boards, toolbars, cards, grids, and panels so hover states and text changes do not shift layout.
- Make mobile layouts intentional, not merely squeezed desktop layouts.
- Ensure text does not overflow buttons, cards, nav items, tabs, or metric tiles.
- Avoid visible instructional text that explains how to use the UI unless the product truly needs onboarding.

## Visual Direction Rules

- Use visual anchors to extract rules, not to copy pixels.
- Translate "premium", "modern", "clean", "playful", or "bold" into concrete choices.
- Avoid one-note palettes dominated by one hue family unless the brief explicitly requires it.
- Avoid decorative blobs, generic gradient orbs, empty bento grids, and stock-like hero sections.
- Use images or product-relevant visuals when a website needs visual assets.
- For SaaS and operational tools, prefer quiet, dense, scannable interfaces over oversized editorial sections.
- For creative portfolios or expressive sites, prioritize a distinct visual point of view while preserving navigation and readability.

## Implementation Rules

- Do not introduce a new UI library, CSS framework, or icon set unless the project already uses it or the user explicitly requests it.
- Do not add abstractions until repeated structure or meaningful complexity justifies them.
- Keep components responsive by design, not through last-minute overrides.
- Include empty, loading, error, selected, hover, focus, and disabled states when the interaction needs them.
- Use accessible labels and keyboard-friendly controls for real actions.
- Treat screenshots as evidence. If the screenshot contradicts the intended style, fix the UI.

## Final Acceptance

Before finishing, verify:

- Desktop viewport looks complete and correctly framed.
- Mobile viewport has no clipped text, hidden controls, or incoherent stacking.
- Primary action is obvious.
- Visual hierarchy matches the product goal.
- The UI does not look like an unstyled template.
- The implementation matches `implementation_brief.md`.
