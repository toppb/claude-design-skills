# Branding and Identity

Type file for brand identity work: naming, positioning, visual identity direction, brand voice.
The core skill (`../SKILL.md`) handles routing, input check, and the overlap and dependency checks.
This file holds the branding-specific work.

**Unit of work:** a brand territory. **Direction:** a territory, meaning a distinct position the
brand could own. **Output:** one HTML board per territory, plus a notes file. This is a direction
round, not final identity design.

**Critical principle:** Territories differ in position and personality, not in color. If two
territories would use the same words and just swap a palette, they are one territory.

---

## Brand 1 — Frame the Brand

Write these down (from the brief, or flag as assumed):

| Item | Question |
|------|----------|
| Business | What they sell, to whom, where, at what price point |
| Audience | Who they want, and what that person cares about |
| Position today | Existing name, logo, customers, reputation, if any |
| Goal | What the brand needs to make happen (premium pricing, trust, launch, differentiation) |
| Constraints | Name fixed or open, budget, applications needed (sign, packaging, web), legal or cultural sensitivities |
| Inspiration | What the client likes and dislikes, and why |

If the scope includes naming, treat naming as its own track inside each territory (Brand 4).

## Brand 2 — Research the Category

Look at 5–8 competitors or adjacent brands, ideally including the local market:
- What do they all look and sound like? That is the category convention.
- Who stands out, and how?
- What position is nobody claiming?

Write the conventions down. Each territory should say whether it follows the convention, or
breaks it, and why that suits this client.

## Brand 3 — Select Territories

Choose 3–5 territories. Build them from the brief and the research, not from a stock list. Use
these axes to make sure they are truly different:

| Axis | Ends |
|------|------|
| Tone | Warm and approachable ↔ Authoritative and precise |
| Stance | Insider, part of the category ↔ Challenger, breaks the category |
| Expression | Restrained and quiet ↔ Expressive and loud |
| Time | Heritage and craft ↔ Modern and forward |
| Audience focus | Speaks to the buyer ↔ Speaks to the user or fan |

Each territory should sit at a different point on at least two axes. Give each a name and a
one-line argument. Examples of the shape (not a menu): "Neighborhood Craft: warm, heritage, local
pride", "Clinical Clean: precise, modern, trust through restraint".

Mark one as recommended, with rationale tied to the goal.

## Brand 4 — Produce the Territory Boards

One HTML board per territory (single self-contained file, inline CSS, no external dependencies).
Each board contains:

1. **Territory name and positioning line**: who it is for, what it stands for, why it is different.
2. **Personality**: three words, each with what it means in practice and what it rules out.
3. **Voice sample**: a headline, a tagline, and a short paragraph written in the territory's voice.
4. **Visual direction** (reference https://styles.refero.design/ for type and palette mood, inspiration only): palette direction (hex values are illustrative; say so in the notes file, not on the board), type direction
   (real font pairings, with why), imagery style, and a logo direction in words, or a simple
   wordmark set in the proposed type.
5. **Applications**: two or three quick sketches or descriptions of the brand in use (sign,
   packaging, web hero), chosen from the client's real needs.
6. **Naming route** (only if naming is in scope): 5–8 candidate names for this territory, each
   with a one-line rationale.
7. **Risks**: what this territory makes harder, and who might dislike it.

**Naming rules:**
- Never state that a name is available, or that a domain or trademark is clear. Availability
  needs a real check (domain registrar, CIPO for Canada, USPTO for the US) and is a dependency
  to flag.
- Check meaning and pronunciation in the languages the audience speaks.
- Include at least one candidate that is descriptive and one that is abstract or evocative.

**Naming of files:** `[project]-brand-[territory-letter]-[territory-name].html`, plus
`[project]-brand-notes.md` with the comparison table, category research and dependency checklist.

## Brand 5 — Overlap Check

Before delivering:
- Any two territories that share personality words or a positioning line? Merge or change one.
- Do voice samples sound different from each other when read aloud?
- Do names repeat across territories?
- Does every territory answer the client's actual goal, not just look good?

## Brand dependencies to flag

Typical blockers: name and domain availability checks, trademark search, client's
must-haves and must-nots, existing assets to keep, application list and sizes, stakeholder who
approves the direction.
