---
name: page-architect
description: >
  Strategic page design and multi-variation HTML wireframing for marketing websites and landing pages.
  Use this skill whenever the user wants to wireframe or architect a homepage, landing page, or any
  marketing website page — even if they just say "mock up the homepage", "show me some layout options",
  "generate wireframe variations", or "let's wireframe the [page name] page". Also use when the user
  shares a client brief, sitemap, or copy document and asks what the page could look like. Produces
  3–5 strategically distinct HTML wireframes with substantive placeholder copy (not gray boxes), kit
  component labels, annotated content dependencies, and production-grade component patterns — ready
  to share with clients for direction and feedback.
---

# Page Architect

Produces 3–5 HTML wireframe variations for a marketing page. Each variation represents a distinct
narrative strategy, uses real placeholder copy grounded in the brief, and annotates what content
is still needed from the client.

**Critical principle:** Wireframe pages as part of a site, not in isolation. Content placement
is a site-wide decision. Every page has a job, and content appears at different depths across
pages. Skipping this step causes overlap, rework, and mid-build confusion.

---

## Step 0 — Site-Wide Content Strategy

**Do this before wireframing any individual page.** If you're wireframing the first page of a
multi-page site, build the content map now. If pages already exist, review them before starting
a new one.

### Define Page Jobs

Every page needs a one-sentence job description that differentiates it from every other page.
If two pages have similar jobs, their content will overlap.

**Example (B2B SaaS):**

| Page | Job |
|------|-----|
| Home | First impression — who we are, what we do, why trust us |
| Platform | How the system works — architecture, methodology, approach |
| Product | What you get — features, UI, workflows, screenshots |
| About | Who built this — team, origin story, values |
| Contact | Convert — form, reassurance, logistics |

If you can't clearly distinguish two pages' jobs, flag it. The architecture needs resolving
before wireframes begin.

### Build the Content Map

Map every content asset to every page. For each cell, assign a **depth level**:

| Depth | Meaning | Example |
|-------|---------|---------|
| **Full** | Complete treatment — this is where the content lives at maximum depth | Testimonials section with 3 quotes on Home |
| **Compact** | Abbreviated version that links to the full treatment | 5-item capability grid on Platform linking to Product |
| **Inline** | Embedded within another section, not standalone | Single testimonial quote inside a feature showcase |
| **Reference** | Name-only or badge/pill linking elsewhere | Framework pills on Product linking to Platform grid |
| **None** | Not on this page | Team bios not on Product page |

**Example content map:**

| Content | Home | Platform | Product | About | Contact |
|---------|------|----------|---------|-------|---------|
| Testimonials | Full (3 quotes) | Full (2 quotes) | Inline (1 contextual) | None | None |
| Frameworks | Reference (logos) | Full (grid + copy) | Reference (pills → /platform) | None | None |
| Capabilities | Compact (3 highlights) | Compact (5 × 1-line) | Full (screenshots per feature) | None | None |
| Screenshots | 1 (hero) | 1–2 (hero, deep feature) | Full set (hero + per-feature) | None | None |
| Team bios | None | None | None | Full | None |
| FAQ | None | Full (architecture-focused) | Full (objection-handling) | None | Compact |

**Rules:**
- Each content asset has exactly ONE page where it appears at **Full** depth
- Other pages use **Compact**, **Inline**, **Reference**, or **None**
- If two pages both need the same content at Full depth, the page jobs aren't distinct enough — fix the architecture
- When content appears on multiple pages, the copy must be different at each depth level (not the same text shortened)

### Differentiate Shared Content

When the same topic appears on multiple pages, vary the angle — not just the length:

| Topic | Platform (approach angle) | Product (feature angle) |
|-------|--------------------------|------------------------|
| Multi-framework mapping | "Why traditional GRC breaks down at 3+ frameworks" | "Implement a control once, map to ISO 27001, SOC 2, PCI-DSS" |
| Evidence collection | "Audit-ready by design — evidence as a byproduct of operations" | "Evidence gathers from cloud infrastructure. Auditors self-serve." |
| Capabilities | Compact overview (name + 1-line, links to Product) | Full deep-dive (screenshot + paragraph per feature) |

---

## Step 1 — Input Check

Before generating anything, assess what you have. Check the conversation and any attached files for:

| Input | Status | Action if missing |
|-------|--------|-------------------|
| Client brief or positioning doc | Required | Use the proposal's Handoff Summary if there is one (see below). Otherwise ask or use whatever exists, flag assumptions |
| Sitemap / page list | Required for multi-page sites | Infer from brief, flag as assumed |
| Approved copy | Optional | Write placeholder copy from positioning; flag clearly |
| Brand voice notes | Optional | Default to professional B2B tone |
| Design system / Figma components | Optional | Extract if available; otherwise use neutral wireframe styles |
| Target audience | Required | Ask if truly unknown |
| Existing wireframes for other pages | Check first | Review before starting to avoid content overlap |

**If a proposal-creator Handoff Summary exists, use it as the brief.** Problem and Success Metrics
set the page jobs. Scope and Phases give the page list. Out of Scope is what not to wireframe. Open
Questions feed the content dependencies in Step 7. Say which fields you used.

**Use the brief's research.** If the brief has Inspiration or Domain notes, read them and say what you
took from each (layout, content order, tone). Skip this if the brief has neither.

**Optional quick scan.** For a new or unfamiliar category, or when the client shared reference sites,
look at two or three competitor or inspiration pages. Note how each orders its content, what it leads
with, and what it leaves out. Use that to pick strategies in Step 2. Don't copy layouts, and don't
let the scan slow down a simple page.

**If wireframes already exist for other pages in the same site**, read them before generating.
Check what content is already placed and at what depth. The new page must complement — not repeat.

State what you found and what you're assuming before generating. Don't ask more than one clarifying
question — make reasonable assumptions and flag them inline with amber warning tags.

---

## Step 2 — Select Narrative Strategies

Choose 3–5 variations from `references/narrative-strategies.md` based on the product and audience.

**Default selection logic:**
- Enterprise B2B SaaS → Trust-First (always), + Problem-First + Feature-Dense
- Consumer or prosumer → Solution-First + Conversion-Minimal + Problem-First
- Early stage / awareness → Problem-First + Solution-First + Trust-First
- High-intent referral traffic → Conversion-Minimal + Solution-First

For each selected strategy, read the corresponding entry in `references/narrative-strategies.md`
for the section sequence and component mapping.

---

## Step 3 — Extract Design System (if available)

If the client has an existing site, landing page, or Figma components, extract the actual design
system before generating wireframes. Don't assume — pull real values.

**What to extract:**
- **Typography:** Font families, weights, sizes for H1–H4, body, captions, code/mono
- **Colors:** Primary, secondary, background tiers (dark, gray, white), text opacity levels
- **Spacing:** Section padding, container max-width, grid gaps
- **Components:** Button styles (radius, padding, variants), card treatments, border styles
- **Containers:** Block types used (dark, bordered, gray, accent) with their CSS properties

**If no design system exists**, use a neutral wireframe aesthetic: system fonts, grayscale palette,
clean editorial styling. The wireframe's job is to communicate structure and copy, not final design.

---

## Step 4 — Write Placeholder Copy

For every text element in every section, write real copy — not "[headline here]" boxes.

Copy must be:
- **Grounded in the brief** — use actual positioning, frameworks, claims from source material
- **Specific, not generic** — "Law 25 and PIPEDA compliance, automated" not "compliance made easy"
- **Clearly flagged as placeholder** — include a note at the top of the file and amber assumption tags on stats, testimonials, and unverified claims
- **Reaction-worthy** — the goal is for the client to say "yes, that direction" or "no, more like X"
- **Depth-appropriate** — copy on a Compact capabilities section reads differently than the Full version on another page. Don't just truncate; reframe for the page's job.

Write headlines, subheads, body copy, button labels, stat figures, feature names, framework names,
FAQ questions/answers, testimonial quotes (with [Company TBD] placeholders), footer link labels.

---

## Step 5 — Generate HTML

Read `references/kit-inventory.md` for the component library reference.
Read `references/component-patterns.md` for component-level best practices, layout patterns, and anti-patterns before writing any HTML. For each component used (Hero, Header, Card, Table, Modal, Navigation, Footer, etc.), apply its documented best practices — sizing, spacing, accessibility, state handling, and anti-patterns to avoid.

**Required elements per section:**
- Green kit label badge (top-left): `Content Left / Layout 1`, `Stats / Layout 2`, etc.
- Amber assumption badge (top-right): when content depends on client delivery
- Assumption note bar (below section): italic amber explanation of what's needed and why

**File structure:**
- Single self-contained HTML file per variation (no external dependencies except system fonts)
- All CSS inline in `<style>` block
- No navigation in wireframes (handled site-wide, above the hero)
- No file chrome, TOC, or summary tables in individual variation files

**Output individual files, not stacked variations.** Each variation gets its own HTML file.
This allows clean Figma capture (one file = one frame) and easier client review.

**Naming:** `[project]-[page]-[variation-letter]-[strategy-name].html`

Example: `acme-platform-a-solution-first.html`

**Additionally**, generate a summary file with the comparison table, content map, and
dependency checklist: `[project]-[page]-wireframe-notes.md`

---

## Step 6 — Deduplication Check

**Before delivering**, run an explicit overlap check against all existing wireframes for the site.

For each content element on the new page, verify:
- Does this content also appear on another page?
- If yes, are they at different depth levels?
- Is the copy angle distinct (not just shorter/longer versions of the same text)?
- Are testimonials reused across pages? If so, is each placement contextually different?

**Common overlap patterns to catch:**
- Same capability names with similar descriptions on two pages
- Same testimonial quote used as both standalone and inline
- FAQ questions that cover the same ground on different pages
- "System of record" or other tagline language repeated verbatim across heroes
- Deep-dive feature sections that duplicate between Platform and Product pages

If overlap is found, resolve it before delivering. The fix is usually:
1. Reduce one page's treatment to a lower depth level (Full → Compact or Reference)
2. Rewrite the copy angle to match each page's job
3. Move the content entirely to one page and remove from the other

---

## Step 7 — Flag Content Dependencies

At the end of the notes file, include a consolidated content checklist. For each item list:
- What's needed
- Which variations require it
- Whether it's blocking (can't build without) or enhancing (can build with placeholder)

---

## Quality Check Before Delivering

- [ ] Site-wide content map exists and is current
- [ ] Page job is defined and distinct from other pages
- [ ] Every section has real copy, not placeholder labels
- [ ] Stats are flagged as illustrative if not from verified source
- [ ] Testimonials use [Name TBD] / [Company TBD] format (or real names if available)
- [ ] No content duplicated at the same depth level across pages
- [ ] Copy angle differs where the same topic appears on multiple pages
- [ ] Each variation is a separate HTML file
- [ ] At least one variation is labeled as recommended with rationale
- [ ] Files open in a browser without errors

---

## Reference Files

- `references/kit-inventory.md` — Figma wireframe kit component catalog (sections, layouts, naming)
- `references/narrative-strategies.md` — 5 strategy definitions with section sequences and component mappings
- `references/component-patterns.md` — 60 UI components with best practices, layout patterns, aliases, and anti-patterns

Read all three before generating. The kit inventory tells you *what components exist*; the narrative
strategies tell you *which ones to use and in what order* for each variation; the component patterns
tell you *how to implement each component correctly* in the HTML output.

---

## Figma Capture Workflow

Individual variation files are designed for Claude Code → Figma capture:

1. Serve files locally: `npx serve .`
2. In Claude Code with Figma MCP installed, prompt:
   "Serve the files in [folder] and capture each HTML page to a new Figma file"
3. Each page lands as a separate editable frame in Figma
4. Text is real text, layout uses auto-layout — ready for design iteration
