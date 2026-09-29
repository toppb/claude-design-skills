# freelance-design-skills

Claude skills for freelance design work, from first brief to approved build. One plugin, `design-workflow`, with four skills:

| Skill | What it does |
|-------|--------------|
| `proposal-creator` | Turns a project brief into a fixed-fee, phased proposal, and produces a Handoff Summary for the next step |
| `design-architect` | Explores 3-5 strategically different directions for a web page or site, a product or app, or a brand. Includes references for web, product UX, branding, and design frameworks |
| `screenshot-to-html` | Rebuilds a product screenshot as an editable HTML file, then renders 1x and 2x PNGs |
| `check-visual` | Verifies a UI change against its reference (Figma, image, live site) before calling it done |

They work in this order: `proposal-creator` -> `design-architect` -> (optional) `screenshot-to-html` -> build -> `check-visual`. Skills hand off through files, and you drive each step.

## Install

```
/plugin marketplace add toppb/freelance-design-skills
/plugin install design-workflow@freelance-design-skills
```

Or copy a skill folder from `plugins/design-workflow/skills/` into your own skills directory.

## Contents

```
plugins/design-workflow/skills/
├── proposal-creator/
├── design-architect/          SKILL.md + references/ (web, product-ux, branding, design-frameworks,
│                              product-patterns, kit-inventory, narrative-strategies, component-patterns)
├── screenshot-to-html/        SKILL.md + scripts/
└── check-visual/
```

## Notes

- `design-architect` includes research notes with sources. Items it could not verify are marked as such in the reference files.
- The wireframe kit reference is based on a free Figma community kit.

## Looking for the resume skill?

It lives in its own repo: https://github.com/toppb/resume-ats-pdf

## License

MIT
