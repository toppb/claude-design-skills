# Product Patterns

Flow and screen patterns for product and app UX, used with `product-ux.md`. Each family lists best
practices and common mistakes, based on Nielsen Norman Group (NN/g), Baymard, GOV.UK Design System,
Apple HIG, Material 3 and W3C guidance. Items marked *unverified* were not confirmed against a
current primary source. Treat patterns as defaults to justify or break, not rules.

---

## Navigation

- Bottom tab bar for a few top-level, equal-weight sections on mobile. Apple's archived iOS HIG says
  3-5 tabs on iPhone, with a "More" tab for overflow (the current HIG may differ, *unverified*).
- Hub-and-spoke for task-focused apps where people do one thing per session.
- Drawer or hamburger only for many options in browse-heavy products. It hurts discoverability of
  primary destinations.
- Sidebar or rail on larger screens (Material 3 pairs a bottom bar on handhelds with a drawer on
  larger devices; destination counts and breakpoints *unverified*).
- Keep tabs visible, and don't disable a tab when its function is unavailable. Tab bars are for
  navigation, not actions.
- **Mistakes:** a hamburger hiding primary destinations, a tab bar used for actions, more than five
  tabs, inconsistent tab context.

## Onboarding and first run

- NN/g's stance: avoid onboarding where possible and fix the UI instead.
- Justified when users must supply information, the app is heavily customised, or features are
  truly novel.
- Customise content (such as language) up front. Leave visual style out, since people can't judge it
  before use.
- Keep instructions short and optional. Prefer contextual help at the point of need.
- Teach with empty states (below).
- **Mistakes:** deck-of-cards tutorials, feature promotion at launch, forcing everything up front.

## Empty, loading and error states

- **Empty:** state the system status, teach with a learning cue, and give a direct action. Never
  leave it blank or treat it as an afterthought.
- **Loading:** 0.1s feels instant, 1s keeps the user's flow, 10s is the limit of sustained
  attention. Skeleton screens for full-page loads of about 2-10s; spinners for single modules;
  progress bars beyond 10s. Skip skeletons under 1s. Animated skeletons can raise accessibility
  concerns.
- **Error:** put the message near its source and don't show it early. Use plain, specific language,
  offer a fix, don't blame the user, and preserve their input.
- **Mistakes:** "no content" followed by populated content, vague instructions, "invalid" wording,
  dismissible toasts for errors.

## Dashboards and data tables

- A dashboard is an at-a-glance view built for quick action. A table supports four tasks: find,
  compare, view or edit one record, and act.
- Freeze header rows and columns in large tables. Make the first column human-readable, not an ID.
- Open one record in a non-modal side panel or edit in place so reference data stays visible.
- Offer batch actions with checkboxes plus per-row actions. Make filters discoverable and column
  hiding or reordering easy.
- Prefer bars, lines and scatter plots on dashboards.
- **Mistakes:** pie or donut charts, treemaps, 3D charts and gauges (NN/g flags them as poor for
  quick reading), modal edit popups that hide the table, horizontal scrolling for comparison.
- No verified source for row density. Don't quote a number.

## Search and filtering

- Autocomplete: about 10 suggestions on desktop and 4-8 on mobile (Baymard). Bold the predicted
  part the user hasn't typed. Style scoped suggestions distinctly. On desktop avoid inner
  scrollbars and support keyboard navigation.
- Filters should be appropriate, predictable, jargon-free and prioritised, with general filters
  first.
- **Mistakes:** vague labels ("Item Type"), internal jargon, missing the filters users need.

## Forms and multi-step wizards

- GOV.UK defaults to one question per page (better focus, lower load, more pages). Group questions
  when they are tightly related. That default comes from a public-services context, so treat it as
  a starting point.
- Never clear fields on error. Write specific error copy that matches the field label, and skip
  "please", "sorry" and "valid/invalid".
- Show an error summary at the top of the page plus a message per field.
- Validate inline when the user leaves the field, not on focus. Clear errors as they're fixed.
- Wizards suit novices and rare tasks, not frequent ones. Show the step list, use descriptive button
  labels, allow save and resume, and make each step self-sufficient.
- **Mistakes:** "This field is required" or "An error occurred" as the whole message, validating
  empty fields early, wizards for routine tasks.

## Settings and account management

No authoritative source was verified for settings organisation or account screens. Apply the shared
principles (descriptive labels, undo for destructive actions) and check Apple HIG and Material 3
directly before making stronger claims.

## Permissions and destructive actions

- Confirm only for serious consequences (destroying work, significant cost). Routine confirmations
  train people to click through.
- Be specific about what will happen, and use action-named buttons ("Delete file" / "Keep file"),
  not Yes/No. Set no default answer.
- For the riskiest actions, require a nonstandard confirmation such as typing a word.
- Go to great lengths to provide undo (NN/g).
- A confirmation dialog that interrupts for a response maps to the W3C `alertdialog` pattern.
- No verified source for roles and permissions UI (role pickers, access tables). Flag as a gap.

## Notifications and feedback

- NN/g separates indicators (contextual status), validations (input errors) and notifications
  (system events).
- Validation errors go inline. Passive notices use a toast or banner. Urgent, action-required items
  use a modal.
- GOV.UK notification banner: use sparingly, one at a time, placed before the page heading, with
  "Success" in the text so meaning doesn't rely on colour alone. Not for validation errors.
- **Mistakes:** wrong channel for the urgency, stacked banners, colour-only meaning, modals for
  frequent updates.
- No verified source for toast timing. Don't quote a duration.

## Mobile and desktop adaptation

Verified points: bottom bar on phone with a drawer on larger devices (Material 3); autocomplete
limits differ (Baymard); tables want persistent headers and a side panel on desktop; tab bars hide
when the keyboard appears (archived HIG). Breakpoints and the exact bar-to-rail-to-drawer
switchover are *unverified*. Check Material 3 window size classes directly.

---

## Screen states every key screen should cover

1. Populated, with realistic data lengths
2. First-use empty, with a cue and an action
3. No results or filtered-empty, with a clear-filters action
4. Loading (skeleton, spinner or progress, chosen by duration)
5. Partial or slow loading *
6. Error: field, page and system level, each with a recovery path
7. Offline or failed request, with retry and preserved input *
8. Success or confirmation
9. Destructive confirmation plus undo
10. No permission or restricted *
11. Disabled or unavailable, with the reason explained *
12. Long content, overflow and truncation *

\* Included by judgment. Not directly confirmed by a source.

## Known gaps

Current Apple HIG and Material 3 numbers (JavaScript-only pages could not be read); settings and
roles and permissions UI; dashboard density; toast timing; breakpoints. The NN/g mobile navigation
article is older and its hamburger stance is contested, so recheck it before relying on it.

## Sources

- NN/g: https://www.nngroup.com/articles/mobile-navigation-patterns/ , /mobile-app-onboarding/ , /empty-state-interface-design/ , /response-times-3-important-limits/ , /skeleton-screens/ , /error-message-guidelines/ , /data-tables/ , /dashboards-preattentive/ , /filter-categories-values/ , /wizards/ , /confirmation-dialog/ , /indicators-validations-notifications/
- Baymard: https://baymard.com/blog/autocomplete-design and https://baymard.com/blog/inline-form-validation
- GOV.UK: https://design-system.service.gov.uk/patterns/question-pages/ , /components/error-message/ , /components/notification-banner/
- Apple iOS HIG (archived): https://codershigh.github.io/guidelines/ios/human-interface-guidelines/ui-bars/tab-bars/index.html
- Material 3: https://m3.material.io/components/navigation-bar/guidelines
- W3C APG alertdialog: https://www.w3.org/WAI/ARIA/apg/patterns/alertdialog/
