# Kit Inventory

Component catalog for the **Wireframes Kit — Free Wireframing Websites and SaaS UI/UX** (Community).
Figma file: `C8zAhhmjoPsjl3nAXKHtVE`

This kit uses a grayscale wireframe aesthetic with Roboto type and IBM Carbon-derived color tokens.
All section components are named `section` in the file — the names below are descriptive labels
derived from their visual structure for use as kit labels in wireframe HTML output.

---

## Design System Tokens

| Token | Value | Use |
|-------|-------|-----|
| `CoolGray/10` | `#F2F4F8` | Page background, alternate section fill |
| `CoolGray/20` | `#DDE1E6` | Borders, placeholder fills |
| `CoolGray/30` | `#C1C7CD` | Dividers, subtle borders |
| `CoolGray/40` | `#A2A9B0` | Placeholder text, inactive icons |
| `CoolGray/60` | `#697077` | Secondary text |
| `CoolGray/90` | `#21272A` | Primary text, headings |
| `Primary/60`  | `#0F62FE` | Primary buttons, active states, links |
| `Primary/90`  | `#001D6C` | Eyebrow labels (uppercase, 20px, bold) |
| `Default/White` | `#FFFFFF` | White section backgrounds |

**Typography:**
| Style | Family | Weight | Size | Line Height |
|-------|--------|--------|------|-------------|
| Heading/1 | Roboto Bold | 700 | 54px | 1.1 |
| Heading/2 | Roboto Bold | 700 | 42px | 1.1 |
| Heading/3 | Roboto Bold | 700 | 32px | 1.1 |
| Body/L | Roboto Regular | 400 | 18px | 1.4 |
| Body/M | Roboto Regular | 400 | 16px | 1.4 |
| Button/L | Roboto Medium | 500 | 20px | 1.0 |
| Caption | Roboto Bold | 700 | 20px | 1.0 (1px letter-spacing, uppercase) |

**Spacing scale:** 8, 16, 24, 32, 48, 64, 80px
**Max content width:** 1280px centered
**Horizontal page padding:** 80px (desktop), 16px (mobile)
**Canvas width:** 1440px desktop, 393px mobile

---

## Button Variants

| Name | Style | Use |
|------|-------|-----|
| `button / primary` | Filled `#0F62FE`, white text, 56px tall, 2px border | Primary CTA |
| `button / secondary` | Outlined `#0F62FE`, blue text, 56px tall, 2px border | Secondary action |
| `button / ghost` | No border, blue text | Tertiary / inline action |

Button label format: `Buttons Group` — always renders as a flex row with 16px gap.

---

## Navigation Components

### Navbars (Desktop)
All named: `Desktop / [Orientation] / [Logo] / [Auth] / [Menu] / [Buttons]`

| Kit Label | Description |
|-----------|-------------|
| `Desktop / Horizontal / logo-left / not-logged / menu-center / buttons-right` | Standard marketing nav — logo left, links centered, CTA right. Height: 80px |
| `Desktop / Horizontal / logo-center / not-logged / menu-left / buttons-right` | Centered logo variant |
| `Desktop / Horizontal / logo-left / not-logged / menu-right / buttons-empty` | Minimal nav, no CTA buttons |
| `Desktop / Vertical / not-logged / buttons-bottom` | Sidebar nav — 256px wide, full height |
| `Desktop / Vertical / logged-in / buttons-bottom` | Sidebar nav with user state |

### Navbars (Mobile)
All named: `Mobile / [Logo] / [Icons]`

| Kit Label | Description |
|-----------|-------------|
| `Mobile / logo-left / two-icons-right` | Standard mobile nav — logo left, hamburger + icon right. Height: 80px |

---

## Section Components

Sections are the primary building blocks. Each is a full-width (1440px) block.
Use these names as the green kit label badges in wireframe HTML output.

### Hero Sections

| Kit Label | Layout | Height |
|-----------|--------|--------|
| `Hero / Split / Content Left / Media Right` | Headline + body + 2 buttons left, screen/video mockup right. `CoolGray/10` background | ~645px |
| `Hero / Split / Content Left / Image Right` | Headline + body + buttons left, illustration or photo right | ~761px |
| `Hero / Centered / Full Bleed` | Large centered headline + subtext + CTA, full-width background image | ~814px |
| `Hero / Centered / Light` | Centered headline + subtext + inline email capture or button, white/light background | ~606px |
| `Hero / App / Download` | Headline + app store badges + app mockup | ~593px |

---

### Feature Sections

| Kit Label | Layout | Height |
|-----------|--------|--------|
| `Features / Icon Grid / 4-col` | Eyebrow + H2 centered, 4 columns of icon + text below, optional CTA. White background | ~532px |
| `Features / Icon Grid / 3-col` | Same pattern, 3 columns | ~496px |
| `Features / Icon Grid / 6-col` | 6 icons in a row, no headline, icon-only strip | ~252px |
| `Features / Content Left / Media Right` | Headline + body + list left, screenshot/mockup right. `CoolGray/10` bg | ~580px |
| `Features / Content Right / Media Left` | Mirror of above — media left, text right | ~580px |
| `Features / Content Left / Stats` | Text + key metrics grid | ~432px |
| `Features / Alternating` | Stacked alternating content-left/right rows | ~580px each |

---

### Social Proof Sections

| Kit Label | Layout | Height |
|-----------|--------|--------|
| `Logos / Bar / Light` | Centered label ("Trusted by") + row of client logos. White bg | ~192px |
| `Logos / Bar / Dark` | Same, dark/charcoal background | ~192px |
| `Testimonials / Grid / 3-col` | 3 quote cards with avatar, name, title, star rating | ~646px |
| `Testimonials / Grid / 2-col` | 2 larger testimonial cards | ~646px |
| `Testimonials / Carousel` | Single featured quote with nav dots, name, company | ~462px |
| `Stats / Band` | Full-width strip of 3–4 large stats with labels. Dark bg | ~205px |
| `Stats / Cards` | 4-column grid of stat cards | ~224px |

---

### Team Sections

| Kit Label | Layout | Height |
|-----------|--------|--------|
| `Team / Grid / 4-col` | Eyebrow + H2 + 4 team member cards (photo, name, title) | ~822px |
| `Team / Grid / 3-col` | Same, 3 columns | ~646px |

---

### Pricing Sections

| Kit Label | Layout | Height |
|-----------|--------|--------|
| `Pricing / 3-tier` | Monthly/annual toggle + 3 tier cards (name, price, feature list, CTA). Standard SaaS pricing | ~957px |
| `Pricing / 2-tier` | 2 larger plan cards with feature comparison | ~743px |
| `Pricing / Comparison Table` | Feature rows × plan columns, checkmarks | ~743px |

---

### Content / CTA Sections

| Kit Label | Layout | Height |
|-----------|--------|--------|
| `CTA / Centered / Light` | Large centered H2 + subtext + button(s). White bg | ~382px |
| `CTA / Centered / Dark` | Same, dark background, white text | ~154px |
| `CTA / Banner / Split` | Text left, button right, full-width band | ~126px |
| `Content / Blog Grid / 3-col` | Eyebrow + H2 + 3 article cards (image, category, title, excerpt, date) | ~993px |
| `Content / Blog Grid / 2-col` | 2 larger article cards | ~681px |

---

### FAQ Sections

| Kit Label | Layout | Height |
|-----------|--------|--------|
| `FAQ / Accordion / 1-col` | Eyebrow + H2 + stacked accordion rows | ~1311px |
| `FAQ / Accordion / 2-col` | Same, split into 2 columns | ~822px |
| `FAQ / List / Simple` | Non-accordion Q&A pairs | ~510px |

---

### Contact / Form Sections

| Kit Label | Layout | Height |
|-----------|--------|--------|
| `Contact / Form / Centered` | Eyebrow + H2 + full form (4 fields + textarea + button) centered, 700px wide | ~684px |
| `Contact / Form / Split` | Contact info left, form right | ~684px |

---

### Footer Components

All named: `Desktop / [Size] / [Logo] / [Layout]`

| Kit Label | Description | Height |
|-----------|-------------|--------|
| `Footer / L / logo-left / subscribe + columns + copy + menu` | Full footer — logo + newsletter signup row, 4 link columns, copyright bar | 578px |
| `Footer / M / logo-left / menu + icons + copy / layout 1` | Medium footer — logo, nav links, social icons, copyright | 180px |
| `Footer / M / logo-left / menu + icons + copy / layout 4` | Variant with different link arrangement | 272px |
| `Footer / S / logo-none / copy` | Minimal footer — copyright only | 68px |

**Mobile footers:**
| Kit Label | Height |
|-----------|--------|
| `Footer / Mobile / L / logo-left / subscribe + columns + copy + menu` | 1302px |
| `Footer / Mobile / M / logo-left / menu + icons + copy / layout 1` | 328px |
| `Footer / Mobile / S / logo-none / copy` | 65px |

---

## Kit Label Convention for HTML Wireframes

Every section in a wireframe HTML file gets a **green kit label badge** in the top-left corner.
Format: `[Category] / [Layout] / [Variant]`

Examples:
- `Hero / Split / Content Left`
- `Features / Icon Grid / 4-col`
- `Logos / Bar / Light`
- `Pricing / 3-tier`
- `FAQ / Accordion / 1-col`
- `Footer / L / Full`

Amber assumption badges go in the top-right when content depends on client delivery.

---

## Common Page Stacks

These section sequences appear across the 7 landing page examples in the kit:

**Standard SaaS Landing Page:**
Nav → Hero/Split → Features/Icon-Grid → Logos/Bar → Features/Content-Left → Features/Content-Right → Stats/Band → Testimonials/Grid → Pricing/3-tier → FAQ/Accordion → CTA/Centered → Footer/L

**Short / High-Conversion:**
Nav → Hero/Centered → Logos/Bar → Features/3-col → CTA/Banner → Pricing/2-tier → Testimonials/Carousel → Footer/S

**Product / App:**
Nav → Hero/App/Download → Features/Alternating → Stats/Cards → Team/Grid → CTA/Centered/Dark → Footer/M
