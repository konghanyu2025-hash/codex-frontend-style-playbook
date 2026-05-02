# GPT Image 2 Anchor Prompt

Use this prompt after `style_brief.md` exists.

```text
Generate 1-3 high-fidelity visual anchors for this frontend. Use Codex image generation with GPT Image 2 if available.

Style brief:
[paste style_brief.md]

The anchors should be realistic frontend screens, not posters, abstract mood boards, or generic template shots.

Each anchor must include:
- visible navigation or screen structure
- real content hierarchy
- primary action
- component density appropriate to the product category
- desktop-safe layout with mobile implications

Avoid:
- copying a known brand
- fake unreadable UI details
- decorative blobs or generic gradients
- oversized empty hero layouts unless the brief asks for a landing page

After generating the images, write visual_anchor.md:
- keep
- reject
- design tokens to extract
- layout rules
- component rules
- responsive implications
- implementation risks
```
