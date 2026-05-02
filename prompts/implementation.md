# Implementation Prompt

Use this prompt after `style_brief.md` and `visual_anchor.md` are complete.

```text
Implement the frontend using the existing project stack.

Inputs:
- style_brief.md
- visual_anchor.md

First write implementation_brief.md with layout, navigation, components, typography, color, imagery, interactions, responsive behavior, accessibility, and QA criteria.

Then implement the UI.

Rules:
- Build the actual requested product screen, not a generic landing page.
- Use the existing component and styling conventions.
- Extract rules from the visual anchors; do not copy pixels.
- Ensure desktop and mobile layouts are both intentional.
- Include realistic states for interactive controls.
- Do not finish until visual QA has been run.
```
