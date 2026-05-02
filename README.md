# Codex Frontend Style Playbook

Codex Frontend Style Playbook is a Codex-first workflow pack for building better frontends with coding agents.

The core idea is simple: do not ask an agent to "make it modern" and hope for taste. First create a visual direction, then extract concrete rules, then implement against screenshot-based acceptance checks.

This repository is not a model, npm package, UI kit, or training dataset. It is a set of reusable agent instructions, workflows, prompts, and examples for front-end work where no exact reference site is provided.

## Why This Exists

Coding agents can reproduce a known website reasonably well when given a strong reference. They often struggle when the request is only a vague style goal, such as "premium", "Apple-like", "clean", or "creative".

This playbook turns vague style intent into implementation constraints:

1. Discover real references.
2. Generate visual anchors with Codex and GPT Image 2.
3. Review those anchors and extract buildable design rules.
4. Implement the actual frontend.
5. Verify with desktop and mobile screenshots.

OpenAI's image generation docs describe GPT Image models including `gpt-image-2`, and show `gpt-image-2` being used through the Image API. See the official [image generation guide](https://developers.openai.com/api/docs/guides/image-generation) and [models page](https://developers.openai.com/api/docs/models).

## Who This Is For

- Codex users who want stronger frontend output.
- Claude Code or other agent users who want a fallback workflow without built-in image quota.
- Maintainers who want a repeatable review standard for AI-generated UI.
- Designers and engineers who need a shared language for style, layout, and visual QA.

## Quick Start

Copy the relevant files into your project, or point your agent at this repository before starting front-end work.

Recommended Codex prompt:

```text
Use this playbook for the frontend work:

1. Read AGENTS.md.
2. Follow workflows/style-discovery.md.
3. Follow workflows/gpt-image-2-anchor.md and generate 1-3 visual anchors.
4. Produce style_brief.md, visual_anchor.md, and implementation_brief.md.
5. Implement the frontend.
6. Follow workflows/visual-qa.md before finishing.
```

If the agent cannot generate images, use the fallback path in `workflows/gpt-image-2-anchor.md`: collect reference screenshots or URLs, then write the same three brief files manually.

## Repository Map

- `AGENTS.md`: default front-end rules for Codex-style agents.
- `workflows/style-discovery.md`: how to turn vague taste into a concrete style brief.
- `workflows/gpt-image-2-anchor.md`: how to generate and review visual anchors.
- `workflows/frontend-implementation.md`: how to turn visual rules into real UI.
- `workflows/visual-qa.md`: screenshot-based acceptance checks.
- `prompts/`: copyable prompts for intake, visual anchors, implementation, and QA.
- `templates/`: blank brief templates for each required output.
- `examples/saas-dashboard/`: example for a dense operational SaaS UI.
- `examples/portfolio-site/`: example for a creative portfolio site.
- `CONTRIBUTING.md`: contribution standards for workflows, prompts, and examples.

## The Three Required Briefs

Every frontend task should produce these files before implementation:

- `style_brief.md`: audience, product type, references, visual intent, information density.
- `visual_anchor.md`: generated or collected visual anchors, what to keep, what to reject.
- `implementation_brief.md`: layout, typography, color, components, responsive behavior, states, and QA criteria.

These briefs are the contract between the visual exploration phase and the coding phase.

## Default Workflow

1. Collect the product goal, users, required screens, key actions, content priority, and brand constraints.
2. Search or list excellent real examples in the same product category.
3. Generate 1-3 visual anchors with Codex and GPT Image 2.
4. Review the anchors and extract buildable rules.
5. Write the three briefs.
6. Build the frontend using the existing project stack.
7. Run desktop and mobile screenshot review.
8. Iterate until there is no obvious layout breakage, text overflow, weak hierarchy, empty hero, or style drift.

## Non Goals

- This is not a replacement for a design system.
- This does not train or fine-tune a model.
- This does not require pixel-perfect reproduction of generated images.
- This does not ask agents to copy copyrighted websites.
- This does not make every project use the same visual style.

## License

MIT
