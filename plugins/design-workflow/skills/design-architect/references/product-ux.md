# Product and App UX

Type file for apps, dashboards, tools and multi-step product experiences (web app, mobile app,
internal tool). The core skill (`../SKILL.md`) handles routing, input check, and the overlap and
dependency checks. This file holds the product-specific work.

**Unit of work:** a flow (a user goal from trigger to done), then the key screens inside it.
**Direction:** a structural model, meaning how the product is organised and how people move
through it. **Output:** a flow map plus HTML wireframes of the key screens, one set per direction.

**Critical principle:** Directions differ in structure, not in styling. Two directions that share a
navigation model and only move buttons around are one direction.

---

## Product 1 — Frame the Problem

Before any direction, write these down (from the brief, or flag as assumed):

| Item | Question |
|------|----------|
| Users | Who, and how often do they come back? Daily tool or occasional task? |
| Core jobs | The 2–4 things people hire this product to do |
| Trigger and success | What makes someone open it, and what does "done" look like? |
| Current state | Existing product, screens or analytics? What is broken, with evidence |
| Constraints | Platform, data and APIs available, accessibility needs, team's build capacity |

If the brief only describes features, ask what job each feature serves. A feature list is not a
brief.

## Product 2 — Define Flow Jobs

Every flow gets a one-sentence job, like page jobs on the web. Map each core job to one primary
flow, and list the flows in priority order. Flows that serve the same job are candidates for
merging. Flows that serve no job are candidates for cutting or for the "out of scope" list.

Also list the **states** each key screen must handle: empty, loading, error, partial data, and
first-run. These are where most product designs fail, so wireframe them for the primary screen of
each direction.

## Product 3 — Select Structural Models

Choose 3–5 directions from this menu, based on user frequency and job type:

| Model | The argument | Fits when |
|-------|--------------|-----------|
| **Task-first (guided)** | One goal at a time, the product leads | Infrequent or high-stakes tasks, onboarding, forms |
| **Hub and spoke** | A home that summarises, with drill-in areas | Several distinct jobs, dashboard-style products |
| **Feed / stream** | Newest or most relevant first, act inline | Monitoring, inboxes, activity, social |
| **Search / command first** | Start from intent, not navigation | Large content or record sets, expert users |
| **Progressive disclosure** | Simple by default, power on demand | Wide skill range between new and expert users |

Default pairings:
- Occasional, non-expert users → Task-first + Progressive disclosure + Hub and spoke
- Daily expert tool → Search / command first + Feed / stream + Hub and spoke
- Subscription or account management → Hub and spoke + Task-first + Progressive disclosure

Write a short entry for each chosen model: the argument, the navigation approach, what the home
screen leads with, and the trade-off it accepts.

## Product 4 — Research

Do a quick audit before choosing. Two or three comparable products (competitors, or best-in-class
for the same job) and the current product if one exists:
- How is it organised and what does the first screen lead with?
- Where do they hide complexity?
- What do they leave out?

Note conventions users will expect, then decide which to follow and which to break, and say why.
Do not copy layouts.

## Product 5 — Produce the Directions

Per direction:
1. **Flow map** for the primary flow: markdown list or Mermaid diagram, with decision points and
   the states above.
2. **3–6 key screens** as HTML wireframes: home or entry, the primary task screen, one
   secondary screen, and the empty and error states of the primary screen.
3. **A short rationale**: the argument, who it serves best, what it makes harder.

Rules for the HTML:
- One self-contained HTML file per screen set (all screens for one direction on one page, stacked
  and labelled), inline CSS, no external dependencies except system fonts.
- Use realistic data. "Invoice 2041 · $1,240 · due in 3 days", not "Item 1". Flag invented data
  with an amber tag.
- Use the client's design system if one exists, otherwise a neutral grayscale wireframe style. For visual polish, https://styles.refero.design/ is an optional reference. Wireframes stay neutral.
- Follow `component-patterns.md` for component behaviour, sizing and accessibility. Read it and
  skip the marketing-only components.
- Mobile-first if the product is used on a phone.

**Naming:** `[project]-[flow]-[direction-letter]-[model-name].html`, for example
`acme-checkout-a-task-first.html`. Plus `[project]-[flow]-notes.md` with the comparison table,
flow maps and dependency checklist.

## Product 6 — Overlap Check

Before delivering, check across directions and across flows:
- Do two directions have the same navigation model? Merge them or change one.
- Does the same screen appear in two flows with different behaviour?
- Do labels for the same action differ between screens?
- Are empty and error states consistent in tone?

## Product dependencies to flag

Typical blockers: real data shapes and API limits, user research or analytics, permissions and
roles, copy for empty and error states, integrations, legal or compliance wording.
