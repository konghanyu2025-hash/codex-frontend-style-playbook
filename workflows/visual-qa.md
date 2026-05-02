# Visual QA Workflow

Use this workflow before delivering any frontend built with this playbook.

## Required Viewports

Check at least:

- Desktop: 1440 x 900.
- Laptop: 1280 x 800.
- Mobile: 390 x 844.

Add more viewports when the product has a known device target.

## Screenshot Review Checklist

Review screenshots for:

- Text overflow.
- Button label clipping.
- Card or panel overlap.
- Navigation collapse issues.
- Hero or first screen emptiness.
- Weak hierarchy.
- Color monotony.
- Excessive decorative elements.
- Inconsistent spacing.
- Missing focus, hover, selected, empty, loading, or error states.
- Important content below the fold without reason.

## Browser Checks

For projects with a dev server:

1. Start the app.
2. Open desktop viewport.
3. Capture screenshot.
4. Open mobile viewport.
5. Capture screenshot.
6. Interact with main controls.
7. Fix visible issues.
8. Repeat until screenshots match the brief.

## Automated Checks

Use Playwright or the project's existing browser test tool when available.

Recommended assertions:

- No horizontal scroll at mobile width.
- Primary nav is visible or intentionally collapsed.
- Primary action is visible.
- No obvious console errors.
- Key controls are keyboard focusable.
- Main content is not blank.

## Visual QA Output

Create or update `visual_acceptance_checklist.md`:

```md
# Visual Acceptance Checklist

## Screenshots Reviewed

## Issues Found

## Fixes Made

## Remaining Risks

## Acceptance Decision
```

## Acceptance Standard

Do not finish if the UI has visible overlapping text, clipped controls, broken mobile layout, blank primary surfaces, or obvious style drift from the implementation brief.
