# Component Patterns Reference

Best practices, layout patterns, and anti-patterns for UI components used in marketing pages
and landing pages. Sourced from component.gallery via ui-design-brain (MIT license).

Components are organized by frequency of use in marketing/landing page contexts.

---

## Core Marketing Components

### Hero
**Also known as:** Jumbotron · Banner

A prominent banner near the top of a page, typically featuring a full-width image or illustration with a headline.

**Best practices:**
- Lead with a compelling headline — clarity over cleverness
- Limit to one primary CTA and optionally one secondary CTA
- Use a high-quality image or illustration that reinforces the message
- Ensure text contrast against the background image (overlay or safe text zone)
- Keep hero height proportional — it should invite scrolling, not dominate the viewport

**Common layouts:**
- Split hero: headline + CTA on left, product screenshot on right
- Full-bleed background image with centered text overlay
- Minimal hero with large headline, subtext, and inline email capture
- Video background hero with centered headline and play button

---

### Header
The persistent top-of-page region containing the site brand, primary navigation, and key actions.

**Best practices:**
- Keep the header height compact (56–72 px) to preserve content space
- Place the logo/brand on the left, primary navigation in the center or right
- Use a sticky header on long pages but consider auto-hide on scroll-down
- Ensure the mobile header collapses into a hamburger menu gracefully
- Maintain clear visual separation from page content (border-bottom or subtle shadow)

**Common layouts:**
- Marketing site header with logo, nav links, and CTA button
- Minimal header with centered logo and hamburger menu

---

### Navigation
**Also known as:** Nav · Menu

**Best practices:**
- Limit primary navigation to 5–7 items; group the rest under 'More' or sub-menus
- Clearly indicate the current/active page in the navigation
- Use consistent iconography alongside text labels for scannability
- Collapse to a hamburger or bottom tab bar on mobile
- Ensure all navigation items are reachable via keyboard (Tab + Enter)

**Common layouts:**
- Horizontal top nav with logo, links, and user menu
- Mega-menu dropdown with categorized link columns

---

### Card
**Also known as:** Tile

A self-contained content block representing a single entity.

**Best practices:**
- Use a single, clear visual hierarchy within each card: media → title → meta → action
- Keep cards a consistent height in grid layouts — use line clamping for variable text
- Make the entire card clickable when it represents a navigable entity
- Use subtle elevation (shadow) or a border — not both simultaneously
- Limit card content to essential info; let the detail page carry the rest

**Common layouts:**
- Feature grid with icon, title, and description
- Pricing tier cards with feature list and CTA
- Blog post feed with thumbnail, headline, excerpt, and date
- Team member directory with avatar, name, and role
- Dashboard KPI cards with metric, delta, and sparkline

---

### Button
An interactive control that triggers an action.

**Best practices:**
- Establish a clear visual hierarchy: primary (filled), secondary (outlined), tertiary (text-only)
- Use verb-first labels: 'Get started', 'Book a demo', not 'Click here' or 'Submit'
- Minimum touch target of 44×44 px; desktop buttons at least 36 px tall
- Show a loading spinner inside the button during async actions
- Limit to one primary button per visible viewport section
- Ensure focus ring is visible and high-contrast for keyboard users

**Common layouts:**
- Hero CTA button centered or left-aligned beneath headline
- Pricing card CTA at the bottom of each tier
- Form submit button aligned right with secondary cancel action

---

### Quote
**Also known as:** Pull quote · Block quote · Testimonial

**Best practices:**
- Use a distinct visual treatment — large quotation marks, left border, or italic text
- Always attribute the quote to its source (name, title, company)
- Keep pull quotes short — they're attention-grabbers, not paragraphs

**Common layouts:**
- Testimonial block with photo, quote, name, and title
- Customer quote in a case study with company logo
- Pull quote in a blog post breaking up long text

---

### Footer
A region at the bottom of a page containing copyright info, legal links, or secondary navigation.

**Best practices:**
- Organize links into clear columns by category
- Include essential legal links: Privacy Policy, Terms of Service
- Keep the footer visually distinct but not distracting — muted background
- Include social links and a newsletter signup if appropriate

**Common layouts:**
- Multi-column footer with link groups, logo, and copyright
- Minimal SaaS footer with product links and social icons
- Single-line footer with copyright and key legal links

---

## Forms & Inputs

### Form
**Best practices:**
- Use a single-column layout for most forms — it's faster to scan
- Place labels above inputs for mobile-friendly forms
- Group related fields with visual proximity and optional fieldset headings
- Show inline validation on blur, not on every keystroke
- Keep forms as short as possible — ask only what's necessary

**Common layouts:**
- Sign-up / contact form with name, email, and CTA
- Multi-step wizard form with progress indicator

---

### Text input
**Best practices:**
- Use appropriate input types (email, tel, url, number) for mobile keyboard optimization
- Show placeholder text only as an example format, never as a label replacement
- Show inline validation errors below the input with a red border and message

---

### Segmented control
**Also known as:** Toggle button group

A compact row of mutually exclusive options for switching views.

**Best practices:**
- Limit to 2–5 segments — more options warrant tabs or a dropdown
- Animate the selection indicator sliding between options
- Use sentence case for segment labels

**Common layouts:**
- Billing period toggle (Monthly / Annually) on pricing pages

---

## Content & Layout

### Accordion
**Also known as:** Collapse · Expandable · Disclosure

**Best practices:**
- Use for long-form content that benefits from progressive disclosure
- Keep headings concise and scannable
- Allow multiple sections open simultaneously unless space is critically limited
- Include a chevron icon aligned consistently on the right
- Animate open/close with a short ease-out transition (150–250 ms)

**Common layouts:**
- FAQ section with stacked question/answer pairs

---

### Tabs
**Also known as:** Tabbed interface

**Best practices:**
- Limit to 2–7 tabs; more options need a scrollable tab bar or overflow
- Clearly indicate the active tab with a bottom border, background fill, or bold text
- Use short, descriptive tab labels (1–2 words)
- Place tab content immediately below the tab bar with no visual gap

**Common layouts:**
- Feature showcase with tabs per capability
- Pricing page with different plan types as tabs

---

### Table
**Best practices:**
- Use a sticky header row for scrollable tables
- Right-align numeric columns for easy comparison
- Alternate row colors (zebra striping) or use horizontal dividers for readability
- Make tables horizontally scrollable on mobile rather than hiding columns

**Common layouts:**
- Pricing comparison table with feature rows and plan columns

---

### Badge
**Also known as:** Tag · Label · Chip

**Best practices:**
- Keep badge text to one or two words
- Use pill shape (fully rounded corners) for status badges
- Avoid overusing badges — if everything is badged, nothing stands out

**Common layouts:**
- Feature label on a pricing tier card (Popular, New, Beta)
- Status indicator (Active, Pending, Archived)

---

### Heading
**Best practices:**
- Use a strict heading hierarchy (h1 → h2 → h3) for accessibility and SEO
- Limit to one h1 per page
- Keep headings concise and descriptive

---

### Separator
**Also known as:** Divider · Horizontal rule

**Best practices:**
- Use subtle, low-contrast separators — they guide the eye, not dominate it
- Prefer spacing over separators when grouping is already clear

---

### List
**Best practices:**
- Use consistent vertical rhythm — equal spacing between list items
- Include dividers between items in dense lists; omit them in spacious ones

**Common layouts:**
- Feature benefit list with checkmark icons
- Activity feed with avatar, description, and timestamp

---

### Image
**Also known as:** Picture

**Best practices:**
- Always provide meaningful alt text for accessibility
- Reserve space for images before they load to prevent layout shift
- Use modern formats (WebP, AVIF) with fallbacks

---

### Video
**Also known as:** Video player

**Best practices:**
- Show a poster/thumbnail image before playback
- Include captions/subtitles for accessibility
- Avoid autoplay with sound

**Common layouts:**
- Product demo video centered on a landing page
- Background video hero with muted autoplay

---

### Carousel
**Also known as:** Content slider

**Best practices:**
- Provide visible navigation arrows and pagination dots
- Support swipe gestures on touch devices
- Auto-advance only if the user hasn't interacted; pause on hover/focus
- Keep slide count manageable (3–7) — carousels with many slides have low engagement

**Common layouts:**
- Testimonial carousel with quote, author, and avatar
- Logo carousel for social proof / partner logos

---

### Progress indicator
**Also known as:** Progress tracker · Stepper · Steps

**Best practices:**
- Clearly distinguish completed, current, and upcoming steps
- Use numbered or labeled steps — not just dots
- Keep the total step count visible so users know the scope

**Common layouts:**
- How-it-works section with numbered steps
- Onboarding or signup wizard

---

### Avatar
**Best practices:**
- Support three sizes: small (24–32 px), medium (40–48 px), large (64–80 px)
- Fall back gracefully: image → initials → generic icon
- For groups, stack avatars with a slight overlap and a '+N' overflow indicator

**Common layouts:**
- Team member card with name and role
- Testimonial block with author photo

---

### Icon
**Best practices:**
- Use a consistent icon style throughout (outlined or filled, not mixed)
- Size icons to align with adjacent text (typically 16–24 px)
- Pair icons with text labels for clarity

**Common layouts:**
- Feature grid with icon + title + description per item
- Navigation item with icon + label

---

### Alert
**Also known as:** Notification · Banner · Callout

**Best practices:**
- Use semantic color coding: red for errors, amber for warnings, green for success, blue for info
- Include a clear, actionable message — not just a status label
- Use an icon alongside color for color-blind accessibility

**Common layouts:**
- Top-of-page banner for announcements (new feature, promotion)

---

### Link
**Also known as:** Anchor · Hyperlink

**Best practices:**
- Make link text descriptive — avoid 'click here' or 'learn more' in isolation
- Underline links in body text for discoverability
- External links should indicate they open in a new tab

---

### Modal
**Also known as:** Dialog · Popup

**Best practices:**
- Use modals sparingly — only for actions requiring immediate attention
- Always provide a clear close mechanism: X button, Cancel, and Escape key
- Trap focus within the modal while it's open

**Common layouts:**
- Demo request / contact form modal triggered by CTA
- Video lightbox for product demo

---

### Tooltip
**Also known as:** Toggletip

**Best practices:**
- Use tooltips for supplementary info — never for essential content
- Show after a short delay (~300 ms) and hide on mouse leave
- Keep tooltip text to a single sentence or a few words

---

## Design System Notes

These principles apply across all components in marketing page contexts:

- **Spacing scale:** Use a consistent spacing scale (4, 8, 12, 16, 24, 32, 48, 64, 96 px)
- **One primary action per section:** Each visible viewport section should have at most one primary CTA
- **Restraint over decoration:** Fewer elements, highly refined. White space is a feature.
- **Typography hierarchy:** Maximize weight contrast between headings and body text
- **Color:** One strong color moment per page; neutral palette for everything else
- **Mobile-first:** Every component should have a defined mobile behavior before desktop
- **Accessibility baseline:** Every interactive component needs keyboard support and ARIA labels
