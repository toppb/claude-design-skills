---
name: design-architect
description: "Strategic design direction for web pages and full websites, product and app UX, and brand identity. Use this skill when the user wants to explore directions before designing: wireframe a homepage or landing page, plan a sitemap, map an app flow, or develop brand territories and naming routes. Also use when the user shares a client brief or proposal handoff and asks what it could look like. Produces 3-5 strategically distinct directions with real placeholder content, annotated dependencies, and a recommendation, ready to share with clients for feedback."
---

# Design Architect

Turns a brief into 3–5 strategically distinct design directions, in the format that fits the
project type. Directions differ in strategy, not styling. Each uses real content grounded in the
brief, and each flags what is still needed from the client.

| Project type | Unit | Direction is a... | Output | Read |
|--------------|------|-------------------|--------|------|
| Web page or full website | Page | Narrative strategy | HTML wireframe per direction | `references/web.md` |
| Product or app UX | Flow | Structural model | Flow map + key screens per direction | `references/product-ux.md` |
| Branding and identity | Brand territory | Position and personality | HTML board per territory | `references/branding.md` |

**Critical principle:** Every unit has one job. A page, a flow or a territory that can't be
distinguished from another by its job will overlap with it. Fix the architecture before producing
directions.

---

## Step 1 — Identify the Project Type

Decide the type from the brief, then read that type's file in `references/` before doing anything
else. State the type in one line.

- A project can mix types (a rebrand plus a new site). Pick the type for the current deliverable,
  say which comes first, and use the previous output as input for the next.
- If the type is unclear, make the most reasonable call and flag it. Ask one question only if a
  wrong guess would waste real work.
- If the request is outside these three types (print collateral, packaging, motion), say so and
  use the core steps below with sensible adaptations, flagging what you improvised.

## Step 2 — Input Check

Before generating anything, assess what you have. Check the conversation and any attached files.

| Input | Status | Action if missing |
|-------|--------|-------------------|
| Client brief or positioning doc | Required | Use the proposal's Handoff Summary if there is one (see below). Otherwise use whatever exists and flag assumptions |
| Scope: pages, flows or deliverables | Required | Infer from the brief, flag as assumed |
| Audience | Required | Ask if truly unknown |
| Approved copy or content | Optional | Write placeholder content from positioning; flag clearly |
| Brand voice, design system, Figma | Optional | Extract if available; otherwise use neutral styles |
| Earlier outputs for the same project | Check first | Review before starting to avoid overlap |

**If a proposal-creator Handoff Summary exists, use it as the brief.** Problem and Success Metrics
set the jobs. Scope and Phases give the pages, flows or deliverables. Out of Scope is what not to
design. Open Questions feed the dependencies in Step 6. Inspiration and Domain Notes feed the
research below. Say which fields you used.

**Use the brief's research.** If the brief has Inspiration or Domain notes, read them and say what
you took from each. Skip this if it has neither.

**Frameworks.** If a framework fits the project (human-centred design, Jobs to Be Done, journey
mapping, WCAG), read `references/design-frameworks.md`, use it, and say which one shaped the work.
Don't claim a framework was followed when only part of it was.

**Quick research.** For a new or unfamiliar category, or when the client shared references, scan
two or three comparable examples (five to eight for branding). Note how each is organised, what it
leads with and what it leaves out. Use that to choose directions. Don't copy, and don't let the
scan slow down a simple job. The type file says what to look for.

**Visual reference (optional).** For visual direction, browse https://styles.refero.design/ (real
sites' design systems by aesthetic: colors, type, spacing, components). Pick two or three that suit
the brief, say what you took from each (a type pairing, a spacing rhythm, a palette mood), and
don't reproduce a specific site. Use it after the directions are chosen, never to choose them.
It's third-party and its terms are unverified, so treat it as inspiration only.

**If earlier outputs exist for the same project**, read them first. The new work must complement,
not repeat them.

State what you found and what you're assuming before generating. Ask no more than one clarifying
question. Otherwise make reasonable assumptions and list them in the notes file. Never mark them on
the mockups.

## Step 3 — Define the Jobs

Write a one-sentence job for every unit (page, flow or territory). If two units have similar jobs,
flag it and resolve it before continuing. The type file has the method (content map for websites,
flow jobs for products, category positions for brands).

## Step 4 — Choose the Directions

Choose 3–5 directions using the selection logic in the type file. Test for distinctness: could a
client tell two directions apart by what they *argue*, not by how they look? If not, replace one.
Mark one direction as recommended, with a rationale tied to the brief's goal.

## Step 5 — Produce the Directions

Follow the type file's output spec. For all types:
- Use real content, grounded in the brief. No "[headline here]" boxes.
- **Keep the mockups clean.** No labels, badges, banners, tags, annotation bars or notes on them.
  The file name carries the strategy. Flag placeholder content, invented numbers and unverified
  claims in the notes file, and write the copy so it reads as real.
- Make it reaction-worthy: the client should be able to say "yes, that direction" or "no, more
  like X".
- One file per direction, so each can be reviewed or captured on its own.
- Also produce a notes file with the comparison table, the recommendation, a list of placeholders
  and unverified items (by section), and the dependency checklist: `[project]-[unit]-notes.md`.

## Step 6 — Overlap Check and Dependencies

**Before delivering**, run the overlap check in the type file across directions and across earlier
outputs.

Then end the notes file with a consolidated dependency checklist. For each item:
- What is needed
- Which directions require it
- Whether it is blocking (can't build without it) or enhancing (can proceed with a placeholder)

---

## Quality Check Before Delivering

- [ ] Project type stated, and the matching type file was read
- [ ] Every unit has a job that is distinct from the others
- [ ] 3–5 directions, each different in strategy, not just styling
- [ ] Real content in every direction, with placeholders and assumptions listed in the notes file
- [ ] Nothing on the mockups except the design itself (no labels, badges, banners or annotations)
- [ ] Overlap check done and resolved
- [ ] One direction recommended, with rationale
- [ ] One file per direction, plus the notes file
- [ ] Dependencies listed and marked blocking or enhancing
- [ ] HTML files open in a browser without errors
- [ ] Anything checkable was checked. Never state that a name, domain or claim is verified unless it was

---

## Reference Files

All in `references/`:

- `web.md` — web pages and full websites: content map, strategy selection, HTML build, Figma capture
- `product-ux.md` — product and app UX: flow jobs, structural models, flow maps, key screens
- `branding.md` — brand identity: category research, territories, boards, naming routes
- `design-frameworks.md` — human-centred design, Double Diamond, Jobs to Be Done, design thinking, heuristics, journey maps, WCAG (all types)
- `product-patterns.md` — flow and screen patterns for product UX: navigation, onboarding, states, tables, forms, search, notifications
- `kit-inventory.md` — Figma wireframe kit component catalog (used by web and product wireframes)
- `narrative-strategies.md` — 5 web page strategies with section sequences and component mappings
- `component-patterns.md` — 60 UI components with best practices, layout patterns and anti-patterns
