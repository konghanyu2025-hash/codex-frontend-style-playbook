# Style Discovery Workflow

Use this workflow before generating images or writing frontend code.

## Inputs

Collect these facts from the task, existing project, or user:

- Product category.
- Target user.
- Primary screen or workflow.
- Required content and actions.
- Brand constraints.
- Information density.
- Device priority.
- Accessibility or localization constraints.
- Existing stack and design system.

If a fact is discoverable in the repo, inspect the repo before asking.

## Product Category Defaults

Use these defaults only when the user gives no stronger direction:

- SaaS or operational tool: dense, restrained, scannable, work-focused.
- Consumer app: clear hierarchy, familiar navigation, strong onboarding path.
- Portfolio: expressive but navigable, with work examples visible early.
- Editorial or content site: typography-led, readable, strong rhythm.
- E-commerce: product-first, inspection-friendly media, clear purchase path.
- Game or interactive toy: visual feedback, motion, and play state clarity.

## Reference Discovery

Find 3-7 high-quality references. Prefer real products in the same category over generic inspiration boards.

For each reference, extract:

- Layout structure.
- Navigation pattern.
- Above-the-fold content priority.
- Typography scale.
- Color behavior.
- Component density.
- Imagery or media treatment.
- Interaction pattern.
- What should not be copied.

Do not copy branded assets, proprietary copy, or unique trade dress.

## Style Brief Output

Create `style_brief.md` with this structure:

```md
# Style Brief

## Product Goal

## Target User

## Required Screens or Sections

## Information Density

## References

## Visual Direction

## Constraints

## Anti Goals
```

## Quality Bar

The style brief is ready only when another agent could understand the intended interface without seeing the original chat.

Reject vague statements like "make it beautiful" unless they are paired with concrete rules.
