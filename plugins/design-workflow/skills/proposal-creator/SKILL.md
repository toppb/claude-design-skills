---
name: proposal-creator
description: >
  Create comprehensive, strategic project proposals for freelance design and consulting work.
  Part of a pipeline: Brief Creator → **Proposal Creator** → One-Pager → PRD. Use when the
  user needs to generate a proposal for a client project. Takes a project brief (or raw context),
  budget, timeline, and rates as input and produces a streamlined, professional proposal document
  with structured handoff data for downstream skills. Triggers on phrases like "proposal",
  "write a proposal", "create a proposal", "scope this project", or "help me price this".
---

# Proposal Creator

Create strategic, comprehensive proposals for freelance projects that position you as a
strategic partner while protecting against scope creep.

**Pipeline position:** This skill sits between the Brief Creator (upstream) and the
One-Pager / PRD generators (downstream).

```
Brief Creator → [you are here] Proposal Creator → One-Pager → PRD
```

---

## Core Principles

These are learned through real project work and are non-negotiable:

1. **Streamline to avoid boxing yourself in** — Keep activities high-level enough that discovery findings can influence your approach. Don't over-specify methods that might not apply.

2. **Focus on problems and goals, not just deliverables** — Frame the proposal around what you're solving, not just what you're making.

3. **Build in protection** — Include revision caps (typically 2 consolidated feedback rounds per phase), clear scope boundaries, and confidentiality clauses.

4. **Structure for parallel work when possible** — Show research/strategy happening alongside critical path items to maintain momentum.

5. **Price proportionally to complexity** — More strategic/complex phases cost more, straightforward execution costs less.

6. **Give yourself flexibility** — Discovery phases should be able to reshape the approach without requiring a complete proposal rewrite.

---

## Pipeline: Input Contract

When receiving input from the Brief Creator, expect these fields. If any are missing,
flag them during the Readiness Check (Step 1 of the workflow).

| Field | Required | Description |
|-------|----------|-------------|
| **Client name** | Yes | Who the proposal is for |
| **Project type** | Yes | UX/Product, Brand/Visual, Web/Landing Page, Consulting |
| **Problem statement** | Yes | What's not working, who's affected, why it matters |
| **Goals & success metrics** | Yes | What success looks like, measurable where possible |
| **Scope signals** | Yes | Pages, features, deliverables mentioned by client |
| **Budget range** | Yes | What the client can spend |
| **Timeline & hard deadlines** | Yes | Launch dates, external dependencies, critical path items |
| **Your rates** | Yes | Standard pricing structure or hourly/weekly rate |
| **Stakeholders** | Recommended | Who's involved, who approves, decision-making structure |
| **Relationship context** | Recommended | Cold lead, referral, existing client — affects tone and format |
| **Domain research** | Optional | Competitive landscape, industry patterns, benchmarks |
| **Supporting materials** | Optional | Emails, chats, docs, audits, briefs |

**If no Brief Creator was used:** Gather these inputs manually in Step 1.

---

## Pipeline: Output Contract

The proposal must produce structured data that downstream skills (One-Pager, PRD) can
consume. After the final proposal is approved, generate a **Handoff Summary** containing:

```
## Proposal Handoff Summary

**Client:** [name]
**Project:** [name / type]
**Problem:** [1-2 sentence problem statement]
**Total Investment:** $[X]K
**Timeline:** [N] weeks ([start] through [end])
**Critical Path:** [what must happen first and why]

**Phases:**
- Phase [N]: [Name] — [objective] — $[X]K — [N] weeks
  - Key deliverables: [list]
  - Dependencies: [what this phase needs or unlocks]
[repeat for each phase]

**Out of Scope:** [explicit exclusions]
**Key Risks:** [top 3]
**Success Metrics:** [primary and secondary]
**Inspiration:** [links the client shared, and what they liked about each]
**Domain Notes:** [anything unfamiliar or researched that later steps should know]
**Open Questions:** [anything unresolved, marked Critical / Important / Nice-to-know]
```

This summary feeds directly into the One-Pager and PRD skills.

---

## Workflow

### Step 1: Readiness Check

Before writing anything, verify you have what you need. Run through the Input Contract
and classify gaps:

- **Critical** (cannot write proposal without this): budget, timeline, problem statement, project type
- **Important** (proposal will be weaker without this): stakeholders, success metrics, domain research
- **Nice-to-know** (can make reasonable assumptions): tool preferences, internal processes, org chart

**Gate:** Do not proceed to Step 2 until all Critical gaps are resolved. For Important gaps,
surface them and let the user decide whether to fill them or accept assumptions.

Present gaps as a synthesis:
> "Here's what I have so far: [summary]. Here's what I'm missing:
> - Critical: [gaps]
> - Important: [gaps]
> - Assumptions I'd make if we proceed: [list]
> Which gaps should we fill before I start structuring?"

### Step 2: Domain Check

**If the client's domain is unfamiliar**, generate a focused research brief before drafting.
This is optional but prevents writing a generic-sounding proposal when you need credibility.

Research areas to consider:
- Competitive landscape (who else does what the client does, and how)
- Industry UX/design patterns and conventions
- Relevant conversion or engagement benchmarks
- User behavior research specific to the domain
- Recent industry shifts that affect the project

You can run this research inline (web search) or generate a standalone research prompt
for deeper investigation.

**Gate:** If domain research surfaces something that changes the project framing (e.g.,
a competitor already solved this differently, or industry benchmarks suggest the client's
targets are unrealistic), flag it before proceeding.

### Step 3: Structure the Project

Based on project type, propose a phase structure:

- Identify what needs to be on the critical path
- Determine if a discovery/research phase is needed
- Plan parallel workstreams if possible
- Flag any phase dependencies

**Present the structure to the user for confirmation before pricing.**

### Step 4: Price It

- Estimate total weeks needed
- Calculate total investment based on user's rates
- Allocate proportionally across phases (see Pricing Strategy below)
- Adjust for complexity, stakeholder count, and risk

### Step 5: Draft the Proposal

Follow the Proposal Structure below. Apply the Clarity Lint (see below) before presenting.

### Step 6: Review & Refine

Walk through key decisions with the user:
- Phasing and critical path
- Pricing allocation
- Scope boundaries and exclusions
- Language and tone

Adjust based on feedback. Finalize document.

### Step 7: Generate Outputs

Produce:
1. **The proposal document** (Google Doc or Word)
2. **The Handoff Summary** (for downstream pipeline skills)
3. **The client email** (see Email Template below)

---

## Clarity Lint

Before presenting a draft, silently check for these. Flag any issues to the user.

**Vague language check** — Flag these words and require specific definitions:
- "modern" → What does modern mean? Clean layout? Current design trends? Specific reference sites?
- "intuitive" → Measurable how? Task completion rate? Time-on-task? Error rate?
- "seamless" → What specifically should feel seamless? Transitions? Data flow? User journey?
- "fast" → Response time target? Page load? Turnaround time?
- "high quality" → Compared to what? What does quality look like for this client?
- "scalable" → Scale to what? 10x users? New markets? Additional features?
- "clean" → Minimal UI? Whitespace-heavy? Specific reference?
- "user-friendly" → For which users? Measured how?
- "robust" → What failure modes does it handle? What's the uptime requirement?

**If vague language appears in client input:** Flag it during the Readiness Check and get
a measurable definition before it goes into the proposal. Don't just pass it through.

**If vague language appears in your own draft:** Rewrite it with specifics or remove it.

**Scope check:**
- Every deliverable mentioned in scope has a corresponding phase
- Every phase has clear deliverables
- Out-of-scope section exists and is specific
- No deliverable appears in multiple phases without explanation

**Protection check:**
- Revision cap language is present
- Assumptions section exists (3-4 items max)
- Timeline assumptions with dependency language included
- Confidentiality clause present

---

## Proposal Structure

All proposals follow this structure. Adapt sections based on project type, but don't
skip sections — mark them N/A with a reason if they don't apply.

### 1. Executive Summary
- Brief context on the challenge
- What you're proposing (3-4 key focus areas)
- **Investment, timeline, start date** (include here, not buried later)

### 2. The Challenge
- Current state (what's not working)
- Technical/business constraints
- Success metrics (primary and secondary) — must be measurable
- Qualitative goals

### 3. Recommended Approach
- Strategic foundation (why this approach)
- What you're doing vs not doing
- How the work is structured (parallel streams, dependencies)

### 4. Scope of Work
- What's included (pages, deliverables, research, strategy)
- What's explicitly out of scope
- Design deliverables (high-level)

### 5. Timeline Overview
- Visual timeline (table format)
- Key milestones
- Important notes on timeline assumptions

### 6. Project Phases
For each phase:
- **Objective:** What this phase accomplishes
- **Activities:** High-level activities (2-4 bullets per section)
- **Deliverables:** Concrete outputs
- **Timeline:** Duration
- **Investment Allocation:** Dollar amount
- **Dependencies:** What this phase needs from the client or previous phases

Phase Structure Guidelines:
- Discovery/Research phase if needed (typically 1-2 weeks, 10-15% of budget)
- Critical path items identified and prioritized
- Strategy/foundation work can run parallel to design work
- Most complex/strategic work gets largest allocation
- Simple execution work gets smaller allocation

### 7. Investment & Payment Structure
- Total investment
- Payment schedule (milestone-based, typically 25% / 30% / 30% / 15%)
- What's included (with revision cap language)
- What requires additional investment

### 8. Process & How We'll Work Together
- Communication (weekly check-ins, async updates, review sessions)
- Feedback & iteration (consolidated feedback, revision caps)
- Tools & access needed

### 9. Success Factors & Risk Mitigation
- What makes this successful (3-4 bullets)
- Potential risks with mitigations (3-4 key risks)
- Assumptions (high-level, 3-4 bullets)

### 10. Why This Approach Works
- Evidence-based / strategic focus / timeline aligned / budget efficient / measurable / sustainable
- Brief bullets, not paragraphs

### 11. Next Steps
- Alignment call
- Contract and initial payment
- Week 1 kickoff plan

### 12. About Me
- Your experience and expertise (2-3 paragraphs)
- **Adapt to project type:**
  - **UX/Product Design:** Focus on UX strategy, conversion optimization, information architecture, user research
  - **Branding/Visual:** Focus on brand strategy, identity design, visual systems, market differentiation
  - **Web/Digital:** Focus on digital experiences, responsive design, user-centered approach
  - **Consulting:** Focus on strategic guidance, business outcomes, collaborative partnership
- Why you're suited for this specific project (connect your experience to their industry/challenge)

### 13. Contact & Confidentiality
- Contact info
- Confidentiality clause: "This proposal is confidential and intended solely for [Client]. It may not be shared with third parties or used for any purpose other than evaluating this engagement."

---

## Streamlining Guidelines

**Activities — Keep High-Level:**
- Bad: "Stakeholder alignment sessions: Review business goals, align on priorities, identify assumptions"
- Good: "Stakeholder alignment and requirements gathering"

- Bad: "Quantitative survey design: Newsletter subscribers discovery path, Instagram followers awareness"
- Good: "Research design (surveys, analytics framework)"

**Why:** Discovery might reveal you need interviews instead of surveys. Don't lock yourself in.

**Deliverables — Combine Related Items:**
- Bad: "High-fidelity mockups, Design rationale annotations, Component specifications, Responsive behavior documentation, Accessibility annotations"
- Good: "High-fidelity mockups (desktop + mobile), Component specifications, Copy direction"

**Why:** Annotations and responsive behavior are implied in quality mockups. Don't over-promise.

**Technical Integration — Stay Tool-Agnostic:**
- Bad: "Vendor-X integration specifications, Vendor-Y event tracking map"
- Good: "Backend integration specifications, Event tracking requirements"

**Why:** Client might switch tools mid-project. Keep language flexible.

**Assumptions — Keep to 3-4 High-Level Points:**
- Bad: Seven detailed bullets about every tool, person, and timeline requirement
- Good: "Access to necessary tools, data, and stakeholders; Timely feedback (within 5 business days); Up to 2 consolidated feedback rounds per phase; Stable technical requirements"

---

## Pricing Strategy

**How to price phases:**

1. **Calculate total based on time:**
   - Estimate total weeks needed
   - Multiply by your weekly rate (or hourly rate x hours/week)
   - This gives you the total investment

2. **Allocate across phases proportionally:**
   - Discovery/Research: 10-15% (if included)
   - Critical path items: 25-30% (typically most strategic work)
   - Strategy/IA work: 15-20%
   - Core design work: 30-35% (largest phase if many pages)
   - Final phase: 10-15%

3. **Adjust based on complexity:**
   - More strategic/uncertain = higher allocation
   - Straightforward execution = lower allocation
   - Backend integration needs = add to allocation
   - Multiple stakeholders = add buffer

**Example phase structure (subscription-media UX overhaul, 12 weeks):**
- Phase 0 (Discovery)
- Phase 1A (Subscription UX — critical path)
- Phase 1B (Strategy & IA)
- Phase 2 (High Priority Pages — most pages)
- Phase 3 (Games & Contests)

---

## Revision Cap Language

**Always include in Assumptions section:**
"Each phase includes up to 2 consolidated feedback rounds. Additional revision rounds beyond this may require timeline and budget adjustment."

**Also in What's Included section:**
"Up to 2 consolidated feedback rounds per phase"

---

## Timeline Assumptions Language

**Always include after timeline overview:**
"The weekly estimates provided are guidelines based on timely responses and feedback. The timeline assumes:
- [Specific dependency 1, e.g., Survey responses within 3-5 days]
- Stakeholder feedback within 5 business days
- [Critical deliverable available Week X]
- Access to tools and data provided promptly

Delays in these areas may extend phase timelines. I'll flag any timeline risks as soon as they emerge and work with [Client] to adjust phases accordingly to maintain project momentum."

---

## Red Flags to Avoid

**Don't:**
- List every single sub-activity (boxes you in)
- Promise specific tools/platforms (they might change)
- Create exhaustive deliverable lists (implies everything else is extra)
- Write 7+ assumption bullets (over-specifies requirements)
- Use "unlimited revisions" language (invites scope creep)
- Make the proposal a contract (it's a conversation starter)
- Add landing page/one-pager for existing relationships (overkill)
- Pass through vague client language without defining it (sounds impressive, means nothing)
- Price before structuring (leads to misallocated budgets)
- Skip domain research for unfamiliar industries (produces generic proposals)

**Do:**
- Keep activities at the right altitude (high-level but clear)
- Stay tool-agnostic where possible
- Combine related deliverables
- Keep assumptions to 3-4 high-level points
- Cap revisions at 2 rounds per phase
- Frame as conversation piece, not take-it-or-leave-it
- Just send email + doc for existing clients
- Lint your own language for vagueness before sending
- Generate the Handoff Summary for downstream skills

---

## Email Template (When Proposal is Ready)

When the proposal is complete, draft an email for the user:

**Subject:** [Project Name] - Proposal

**Body:**
```
Hi [Client Name],

I've put together a proposal based on the project brief. The approach addresses the core
challenges and goals you outlined, while keeping [critical deadline/constraint] on the
critical path.

Here's the proposal: [Google Doc link]

Key highlights:
- $[X]K investment across [N] phases
- [Timeline] ([start] through [end])
- [Critical deliverable] delivered [date] for [reason]
- All [scope items] from the brief included

I'd love to hop on a quick call to walk through it and answer any questions. The approach
is flexible — if certain phases need adjustment based on priorities or budget, we can
definitely discuss.

When works for a 30-min chat?

Best,
[User Name]
```

**Keep it:** Professional but conversational. Focused on their needs. Inviting discussion.
Brief with key info in bullets.

**Voice:** If the user has a voice or style skill, run the email through it before handing it over. The template above is a structure, not the wording. Open with one short, specific line, not a summary of the proposal.

---

## Common Adjustments After Client Feedback

**If they want to cut scope:**
- Ask what's lowest priority
- Remove that phase or reduce deliverables
- Adjust pricing proportionally
- Explain impact on outcomes

**If they want to add scope:**
- Estimate additional weeks needed
- Calculate additional cost proportionally
- Explain timeline impact
- Update proposal with new scope

**If budget is too high:**
- Offer to reduce scope to hit budget
- Show what would be cut and impact
- OR explain value and hold firm
- OR meet in middle by streamlining slightly

**If timeline is too long:**
- Identify what can run in parallel
- Ask if they can provide resources faster
- OR explain why timeline is realistic
- Don't compress unrealistically just to win work

---

## Adaptation Guidelines

**Brand/Visual Design Projects:**
- Focus on deliverables (logo, guidelines, templates)
- Less emphasis on discovery/research
- More emphasis on revision rounds for creative work
- Shorter timelines typically

**Strategic UX/Product Design Projects:**
- Heavy discovery/research phase (like the subscription-media example above)
- Focus on IA, strategy, conversion optimization
- Multiple parallel workstreams
- Longer timelines, more complex

**Website/Landing Page Projects:**
- Simpler phase structure (Discovery → Design → Handoff)
- Clear page counts and deliverables
- Less strategy emphasis unless needed
- Shorter timelines

**Consulting/Retainer Work:**
- Different pricing structure (monthly retainer)
- Focus on ongoing support vs project deliverables
- Scope by hours or activities per month
- Rolling engagement vs fixed timeline

Adapt the structure, but keep the core principles consistent across all project types.

---

## Success Criteria

A good proposal:
- Positions you as strategic partner, not order-taker
- Focuses on solving problems, not just making things
- Protects you from scope creep (revision caps, clear exclusions)
- Gives you flexibility to adapt based on discovery
- Is appropriate for the relationship (doc for existing clients, more context up front for cold leads)
- Invites discussion rather than demanding approval
- Prices fairly based on your rates and project complexity
- Includes confidentiality protection
- Feels professional but not overly formal
- Is scannable (bullets, tables, clear sections)
- Contains no vague language that hasn't been defined
- Produces a clean Handoff Summary for downstream skills

---

## Example: Subscription-media UX overhaul

For reference, here's how these principles were applied to a real UX overhaul project:

**Context:**
- Referred client (existing relationship)
- Timeline: 12 weeks with critical launch deadline for subscription UX
- Major backend transformation happening (new customer-data stack)
- 5 stakeholders plus light involvement from founder

**Key Decisions:**
- Positioned as strategic UX overhaul (IA, messaging, conversion) not visual redesign
- Discovery phase (2 weeks) to validate approach before committing to design direction
- Subscription UX prioritized on critical path (Weeks 3-5) to hit the deadline
- Strategy/IA ran parallel to subscription work to maintain momentum
- Fixed fee split across 5 phases
- Streamlined activities to avoid locking into specific methods
- Kept technical specs tool-agnostic (not a named-vendor spec but "backend integration specs")
- Included 2-round revision cap with 5 stakeholders to prevent conflicting feedback
- Sent as Google Doc + email (not landing page) since existing relationship
- Added confidentiality clause to protect strategy if they shopped around

**Result:**
- Professional, comprehensive proposal
- Protected against scope creep
- Flexible enough for discovery to reshape approach
- Positioned strategically vs transactionally
- Ready to negotiate if needed

---

**Remember:** The proposal is a conversation starter, not a contract. Be professional,
be strategic, but be ready to discuss and adjust.
