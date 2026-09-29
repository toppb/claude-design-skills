# Design Frameworks

Process frameworks to lean on when framing a project, choosing directions and checking the result.
They apply to all three project types. Use them as lenses, not ceremony: name the one or two that
fit, say how they shaped the work, and skip the rest. Don't claim a framework was followed if only
part of it was (for example, don't call a project "human-centred" if no users were involved).

Sources were checked in a research pass. Items marked *unverified* were not confirmed against a
primary source.

---

## Quick pick

| Framework | Web | Product / app | Brand | Plugs in at |
|-----------|-----|---------------|-------|-------------|
| Human-centred design (ISO 9241-210) | Light | Core process | Weak | Brief, evaluation |
| Double Diamond | Phasing | Phasing | Phasing | Proposal |
| Jobs to Be Done | Brief, copy, IA | Brief, requirements | Brief, positioning | Brief, jobs |
| Design thinking | Rarely | Early concepting | Naming and territory workshops | Directions |
| Nielsen's 10 heuristics | Review | Prototype review | n/a | Before delivery |
| Journey map / service blueprint | Multi-step only | Strong fit | Rare | Flow jobs |
| WCAG 2.2 (POUR) | Baseline | Baseline | Palette contrast only | Build, QA |

---

## Human-centred design (ISO 9241-210:2019)

A process standard for interactive systems, not a UI checklist.
- **Principles:** design rests on understanding users, tasks and environments; users are involved
  throughout; design is driven by user-centred evaluation; the process is iterative; it addresses
  the whole user experience; the team has multidisciplinary skills.
- **Four activities (iterative):** understand and specify the context of use; specify user
  requirements; produce design solutions; evaluate the design.
- **Use when:** you want low-ceremony rigour on a product or app project. Treat it as a checklist:
  context, requirements, solutions, test.
- **Don't:** cite it as formal compliance, or call the project human-centred when no users were
  reachable. Say what was and wasn't tested.
- **Verification note:** the standard itself is paywalled. This is based on a free sample of the
  2019 text and a secondary source; section numbers were not checked against the full standard.

## Double Diamond (Design Council)

Two diverge-then-converge cycles: find the right problem, then the right solution. Stages:
Discover, Define, Develop, Deliver. It is not linear, and teams loop back.
- **Use when:** you need a simple client-facing story to phase and price a proposal.
- **Don't:** present it as a method. It has no techniques of its own, and on a small fixed-scope job
  it is overkill.
- **Verification note:** Design Council's page dates the model to 2003 (other sources say 2005, so
  the date is disputed). The 2019 Framework for Innovation adds four principles (put people first,
  communicate visually and inclusively, collaborate and co-create, iterate) and a methods bank. What
  changed from the earlier model was *unverified*.

## Jobs to Be Done

Customers "hire" a product to make progress in a situation. Study circumstances and motivation, not
demographics.
- **Job story format:** "When [situation], I want to [motivation], so I can [outcome]." Its origin
  (often credited to Intercom) is *unverified*.
- **Two schools, which disagree:** Christensen and Moesta are qualitative, built on switch
  interviews (push, pull, anxiety, habit). Ulwick's Outcome-Driven Innovation is quantitative: job
  steps, outcome statements, and survey scores of importance against satisfaction.
- **Use when:** writing a brief or positioning and pinning down why people choose the client's thing.
  A few customer interviews plus job stories is realistic for a small client.
- **Don't:** aim for statistical validity on a small budget (ODI needs real resources), or expect
  help with visual or interaction detail.

## Design thinking (Stanford d.school, IDEO)

Empathize, Define, Ideate, Prototype, Test, not strictly linear. NN/g adds a sixth stage, Implement.
- **Use when:** the problem is vague and you need concepts fast: naming or brand workshops, early app
  ideas. Paper or Figma prototypes keep it cheap.
- **Don't:** use it when scope is already defined (a template-based site) or the client can't make
  time for workshops.

## Nielsen's 10 usability heuristics (NN/g, reviewed Jan 2024)

Visibility of system status; match between the system and the real world; user control and freedom;
consistency and standards; error prevention; recognition rather than recall; flexibility and
efficiency of use; aesthetic and minimalist design; help users recognise, diagnose and recover from
errors; help and documentation.
- **Use when:** you need a fast expert review of a prototype or an existing site, or a structure for
  audit findings in a proposal.
- **Don't:** treat it as test results. It finds likely problems, not proof, and it doesn't cover
  accessibility compliance or brand quality.

## Journey maps and service blueprints (NN/g)

A journey map is a timeline of what one actor goes through to reach a goal: phases, actions,
mindsets and emotions, opportunities. A service blueprint adds the layers behind it: customer
actions, frontstage actions, backstage actions, support processes.
- **Use when:** the experience has several steps or crosses channels (booking, onboarding), or the
  team needs a shared view. Blueprints suit services with real back-office steps.
- **Don't:** map from guesses (maps need research to be credible), use them for simple linear sites,
  or use them as implementation detail. NN/g points to user-story maps for development planning.

## WCAG 2.2 (W3C, Recommendation December 2024)

Organised by four principles: Perceivable, Operable, Understandable, Robust. Levels A, AA, AAA. 2.2
adds nine success criteria and removes 4.1.1 Parsing.
- **Use when:** on every web or app build. Target AA as the baseline. Check contrast, focus states,
  target size, forms and alt text during design and QA.
- **Don't:** treat it as a substitute for usability testing, or claim legal compliance without a real
  audit. Print and identity work is largely out of scope, apart from colour contrast in palettes.

---

## How directions use these

- **Brief and input check:** JTBD for why people choose the client; the ISO "context of use"
  activity; a journey map if the experience has real steps.
- **Proposal:** Double Diamond to phase and price the work, in plain language for the client.
- **Directions:** design thinking for concepts; journey maps to support flows.
- **Before delivering:** a heuristic pass on any product or web wireframe, and WCAG AA checks on
  contrast, focus, target size and forms.
- Say in the notes file which frameworks shaped the work and which were skipped, and why.

## Sources

- ISO 9241-210:2019 sample: https://cdn.standards.iteh.ai/samples/77520/8cac787a9e1549e1a7ffa0171dfa33e0/ISO-9241-210-2019.pdf
- Design Council: https://www.designcouncil.org.uk/our-resources/the-double-diamond/ and https://www.designcouncil.org.uk/our-resources/framework-for-innovation/
- JTBD: https://gopractice.io/product/jobs-to-be-done-the-theory-and-the-frameworks/ and https://strategyn.com/jobs-to-be-done/
- d.school: https://dschool.stanford.edu/resources/design-thinking-bootleg and NN/g: https://www.nngroup.com/articles/design-thinking/
- NN/g heuristics: https://www.nngroup.com/articles/ten-usability-heuristics/
- NN/g journey maps: https://www.nngroup.com/articles/journey-mapping-101/ and blueprints: https://www.nngroup.com/articles/service-blueprints-definition/
- W3C: https://www.w3.org/WAI/WCAG22/Understanding/intro and https://www.w3.org/TR/WCAG22/
