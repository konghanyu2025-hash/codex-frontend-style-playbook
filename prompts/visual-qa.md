# Visual QA Prompt

Use this prompt after implementation.

```text
Run visual QA for the frontend.

Check at least:
- 1440 x 900
- 1280 x 800
- 390 x 844

Review for:
- text overflow
- clipped controls
- overlapping panels
- broken navigation
- weak hierarchy
- blank primary surfaces
- color monotony
- style drift from implementation_brief.md

Capture or inspect screenshots. Fix issues and repeat until the UI meets the brief.

Write visual_acceptance_checklist.md with screenshots reviewed, issues found, fixes made, remaining risks, and acceptance decision.
```
