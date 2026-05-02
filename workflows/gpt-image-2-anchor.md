# GPT Image 2 Visual Anchor Workflow

Use this workflow after `style_brief.md` exists and before frontend implementation begins.

## Goal

Generate 1-3 visual anchors with Codex and GPT Image 2, then extract practical design rules from those images.

The images are not the final product. They are visual evidence for layout, proportion, density, color, and mood.

## Codex Main Path

Ask Codex to generate 1-3 visual anchors. Each anchor should represent a different viable direction while staying inside the style brief.

Use this prompt shape:

```text
Generate a high-fidelity frontend style exploration image for this product.

Product:
[product summary]

Audience:
[target user]

Screen:
[screen or site section]

Style constraints:
[visual direction from style_brief.md]

Must show:
[required content and actions]

Avoid:
[anti goals]

Output should look like a real responsive web product, not a mood board, not a poster, and not a generic template.
```

## Fallback Path

If GPT Image 2 is unavailable:

1. Collect 3-7 reference screenshots or URLs.
2. Write a short visual summary for each.
3. Choose one primary direction and one backup direction.
4. Continue with the same `visual_anchor.md` structure.

## Review Each Anchor

For each generated or collected image, identify:

- What layout ideas are buildable.
- What color and contrast behavior is worth keeping.
- What typography scale is visible.
- What component shapes and density are useful.
- What imagery or media treatment is relevant.
- What is decorative noise.
- What cannot be implemented responsibly.
- What would fail on mobile.

## Visual Anchor Output

Create `visual_anchor.md` with this structure:

```md
# Visual Anchor

## Inputs

## Anchor Images

## Keep

## Reject

## Design Tokens to Extract

## Layout Rules

## Component Rules

## Responsive Implications

## Implementation Risks
```

## Hard Rules

- Do not implement directly from the image.
- Do not copy text, logos, or unique branded assets from references.
- Do not preserve unrealistic UI details that only look good in a static image.
- Do not accept an anchor that has no clear navigation, hierarchy, or real content.
