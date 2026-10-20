---
name: Home Again Cleaning Services
description: Calm band pitch site for a locally owned Ocean County, NJ cleaner; paper, two harbour navies, one sparkle gold.
colors:
  sparkle-gold: "#f5c64f"
  sparkle-gold-light: "#ffd877"
  gold-ink: "#7f5a00"
  harbour-navy: "#1f4a7a"
  deep-navy: "#10233f"
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  ink: "#10233f"
  body: "#2a3a4c"
  soft: "#4a5868"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d7ea"
  line: "rgba(16,35,63,.12)"
  focus: "#1f4a7a"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-.005em"
  display-desktop:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "96px"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(20px, 5.4vw, 24px)"
    fontWeight: 400
    lineHeight: 1.15
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(18px, 4.8vw, 20px)"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1
  wordmark-desktop:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "25px"
    fontWeight: 400
    lineHeight: 1
rounded:
  focus: "6px"
  field: "10px"
  panel: "16px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-desktop: "40px"
  section-y: "64px"
  section-y-desktop: "96px"
  container: "1160px"
components:
  button-primary:
    backgroundColor: "{colors.sparkle-gold}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.sparkle-gold-light}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-checked:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  float-circle:
    backgroundColor: "{colors.sparkle-gold}"
    textColor: "{colors.ink}"
    size: "60px"
---

# Design System: Home Again Cleaning Services

## Overview

**Creative North Star: "The Harbour Porch Light"**

A calm, warm home for a small local cleaner: an off-white page cut into full-bleed bands of harbour navy and deep navy, with one sparkle gold doing every warm job. Nothing on the page claims more than the business has. There are no photos, no logo, no reviews, so the system carries trust through colour, generous spacing, soft shapes and one confident display face. The gold comes from the sparkle in the owner's own post and is used the way a porch light is: one warm point on a dark ground, there to tell you where to go.

Density is low and phone-first. Each band holds one idea: who and where (hero), why trust them (care), what they clean (services), how to ask (estimate), and who they are (close). Shapes are borderless and rounded; depth comes from band contrast, not shadows. Motion is limited to a single hero entrance, a single quiet fade-up for content below the first screen, and small state feedback.

This build follows the pitch-site calm band style (lpmr.co.uk lineage) in its no-photo variant: the hero is the navy band with the diagonal line texture because no client photo exists.

**Key Characteristics:**
- Full-bleed bands alternate paper and navy so every new section is obvious.
- One warm accent, gold, used as a fill; text on gold is always ink navy.
- One display webfont (Cal Sans) for headings, buttons, labels and list rows; system stack for running text.
- Soft, borderless geometry: 24px cards, 10px fields, full pills.
- Flat surfaces; the only shadow belongs to the floating message circle.
- Every contact point is wired through one config switch (Messenger today, call/text once a phone is set).

## Colors

Paper, two harbour navies and one sparkle gold; a restrained palette where the accent's rarity is what makes it a signal.

### Primary
- **Sparkle Gold** (sparkle-gold): the one warm accent. Fills only: primary buttons, the floating message circle, the hover/focus fill on service-row arrows, the eyebrow dot, text selection. On dark bands it also colours the last phrase of a heading.
- **Sparkle Gold Light** (sparkle-gold-light): hover state of gold fills only.
- **Gold Ink** (gold-ink): gold when it must be text or an icon on a light ground (the accent phrase on paper, the claim icons). It exists because gold on paper fails contrast.

### Secondary
- **Harbour Navy** (harbour-navy): the hero band and the closing band; also the focus/hover outline on light grounds, the caret colour, and the header contact icon.
- **Deep Navy** (deep-navy): the services band and the footer, always with the diagonal line texture. Shares its value with Ink by design: the darkest band and the heading colour are the same navy.

### Neutral
- **Paper** (paper): page ground, header, and the light bands (care, estimate). Never black, never pure white.
- **Card** (card): the estimate form card and the copied-message box; the only pure-white surface.
- **Field** (field): tinted fill for inputs, unchecked chips and the post-send panel.
- **Ink** (ink): headings and all text on gold.
- **Body** (body): running text on light.
- **Soft** (soft): secondary text on light (ledes, hints, placeholders, wordmark subline).
- **On Dark / On Dark Soft** (on-dark, on-dark-soft): headings and running text on navy bands respectively.
- **Line** (line): hairline dividers between claim rows on paper. On dark bands the equivalent divider is `rgba(255,255,255,.12)`.
- **Error** (error): validation border and message text only.

### Named Rules
**The Porch Light Rule.** Gold is a fill, never text on a light ground. Text on gold is Ink; gold-as-text on paper switches to Gold Ink. Gold-as-text appears only on navy bands.

**The One Warm Point Rule.** Each viewport carries at most one gold call to action (plus the floating circle, which hides whenever the form or the closing button is on screen). Gold is not used for decoration beyond the eyebrow dot and the dark-band accent phrase.

**The Band Contrast Rule.** Sections are separated by full-bleed colour change, not borders or cards: paper header, navy hero, paper, textured deep navy, paper, navy, textured deep navy footer.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui fallback), loaded from Google Fonts with preconnect, weight 400 only.
**Body Font:** system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial).

**Character:** a rounded, friendly geometric display face that does all the speaking parts (headings, buttons, list rows, form labels), paired with a native system body that disappears into the phone.

### Hierarchy
- **Display** (400, clamp(42px, 12vw, 80px), 96px from 1024px, line-height 1.02, max 11ch / 14ch on desktop): the hero H1 only, white on navy, last phrase in gold.
- **Headline** (400, clamp(30px, 7.6vw, 48px), 1.08, balanced wrap): every section H2.
- **Title** (400, clamp(20px, 5.4vw, 24px), 1.15-1.2): claim rows, service rows (to 23px), numbered steps (22px).
- **Lede** (system 400, clamp(18px, 4.8vw, 20px), 1.5 for the hero promise, 1.7 elsewhere, 32-40ch): the line under a headline.
- **Body** (system 400, 16px, 1.7): running text, inputs (never below 16px so iOS does not zoom), footer.
- **Label** (Cal Sans 400, 18px, line-height 1): buttons, form labels and legends, header contact link (20px desktop).
- **Wordmark** (Cal Sans 22px / 25px desktop over a system 600 12px uppercase 0.08em subline): the header brand only.

### Named Rules
**The One Voice Rule.** Cal Sans at weight 400 is the only display voice; hierarchy comes from size, never from bold display weights or a second display face.

**The 16px Floor Rule.** Nothing interactive or readable is set below 16px except the 12px wordmark subline and 14px optional-field hints.

## Layout

A single centred container (max 1160px) with a 20px gutter on phones and 40px from 760px. Sections are full-bleed bands with 64px vertical padding on phones and 96px from 760px. The hero has its own padding (56/64px, rising to 96/112px on desktop screens at least 600px tall).

Breakpoints: 760px (gutter, section padding, hero buttons go side by side at min 240px wide), 1024px (two-column splits). From 1024px the care band becomes a 1fr/1fr split with 64px column gap, the services list becomes two columns, the estimate band becomes 1fr/1.2fr with the heading block sticky at 40px from the top, and the close band aligns its button to the bottom right.

Rhythm is loose and list-driven: content sits in stacked rows separated by hairlines rather than in card grids. Headline blocks cap at 640px; ledes at about 40ch. The footer reserves bottom padding (96px plus safe area) so the floating circle never covers its links. Safe-area insets are respected in the header, footer and floating circle.

## Elevation & Depth

The system is flat. Depth is conveyed by band colour contrast and by the white form card sitting on paper. The diagonal line texture (`repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`) is the only surface treatment and appears on the hero, the services band and the footer, never on the mid-navy close band.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(8,24,46,.3)`): the floating message circle only, because it sits over every band.
- **Pick pulse** (animated ring `0 0 0 0 rgba(31,74,122,.55)` to `0 0 0 12px rgba(31,74,122,0)`, 0.9s ease-out, once): the chip pre-selected when a service row sends the visitor to the form. State feedback, not elevation.

### Named Rules
**The Flat Band Rule.** No surface casts a shadow at rest except the floating circle. Cards and buttons are separated by fill, not lift.

**The Faint Texture Rule.** The line texture stays at about 3.5% white or fainter so it never reads as lines through text.

## Shapes

Soft and borderless. Three radii only: 10px for text fields, 24px for the form card (16px for the inner post-send panel), and full pills for buttons, chips and the eyebrow. Circles for the service-row arrows (44px), the numbered step discs (44px) and the floating circle (60px). Inputs and chips carry a 2px transparent border that only takes colour on hover, focus or error, so state never shifts layout. Icons are inline SVG line drawings at 2.2-2.6 stroke with round caps and joins.

## Components

### Buttons
Big, round and calm.
- **Shape:** full pill (999px), min height 56px, 26px side padding, Cal Sans 18px, optional 20px leading icon.
- **Primary:** Sparkle Gold fill and border, Ink text. Hover lightens to Sparkle Gold Light.
- **Ghost:** transparent with a 70% on-dark outline, on navy only; hover goes to a white outline over 10% white. Inside the post-send panel on light it inverts to an Ink outline.
- **Press:** scale(.98) over 0.12s. Colour transitions 0.2s. Hover styles exist only under `(hover:hover)`.
- **Focus:** 3px outline offset 3px; navy on light, gold on navy bands. Full-width inside the form.
- At most two in the hero (primary + ghost); no Call button in the hero.

### Chips
- **Style:** pill on Field fill, 48px tall, system 16px Ink text, visually hidden radio behind each.
- **State:** hover/focus colour the 2px border navy; checked flips to an Ink fill with white text.

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** Card white on paper.
- **Shadow Strategy:** none (see Flat Band Rule).
- **Internal Padding:** clamp(20px, 5vw, 32px), 22px gap between fields, max 600px wide.

### Inputs / Fields
- **Style:** Field fill, no visible border, 10px radius, 52px min height (textarea 112px, vertical resize), system 16px Ink text, navy caret, Soft placeholder.
- **Labels:** Cal Sans 18px Ink above the field; optional fields get a 14px Soft "(optional)" hint.
- **Focus / Hover:** 2px border turns Harbour Navy; no glow.
- **Error:** border turns Error red and a 16px plain-language message appears below; validation runs on submit only and clears as the visitor fixes the field.

### Navigation
- **Header:** paper strip, wordmark left, one contact link right (Cal Sans 18/20px with a navy icon; hover turns the text navy). 64px tall, 76px from 760px. No menu.
- **Footer:** textured deep navy, copyright plus contact links at 44px tap height; hover turns links gold.

### Service Rows (signature)
Each service is a full-width link row on the textured deep navy band: Cal Sans 20-23px on-dark text, 72px min height, white 12% hairlines between rows, a 44px circular arrow on 10% white at the end. On hover or focus only the arrow changes (gold fill, Ink arrow; focus adds a gold ring). Clicking a row scrolls to the form, pre-checks the matching chip and pulses it once.

### Claim List
Rows of Cal Sans 20-24px Ink text on paper, each led by a 40px Gold Ink line icon, divided by Line hairlines. Used instead of feature cards.

### Numbered Steps
A three-step ordered list beside the form: 44px circular discs on 8% ink with a Cal Sans counter, Cal Sans 22px step text.

### Floating Message Circle (signature)
One 60px gold circle bottom-right with an Ink icon and the Float lift shadow; never a bottom bar. It slides up from 120px below (0.35s cubic-bezier(.2,.8,.2,1)) once the hero leaves view and slides away while the form or the closing button is on screen. It is removed entirely when `CONFIG.FLOAT` is false or IntersectionObserver is missing.

### Contact Wiring
Every contact element carries `data-reach` and is pointed at `CONFIG.MESSENGER` on load. Setting `CONFIG.PHONE` (and optionally `CONFIG.PHONE_LABEL`) switches the whole system in one place: header link becomes `tel:` with the phone icon and the number, the close button and floating circle become `sms:` with a prefilled body and the chat icon ("Text us"), the form button becomes "Text this to us" and sends the composed message by SMS, and the footer gains the number. Without a phone, the form composes the message, copies it, and reveals a panel (Field fill, 16px radius) with the message in a white box, an "Open Messenger" primary button and a "Copy message again" ghost button. Editing the form after that hides the panel so a stale message is never sent. New contact surfaces must join this wiring rather than hard-coding a link.

### Motion
- **Hero H1 bounce-in:** hero H1 only. JS splits it into letters inside nowrap word spans; each letter goes from opacity 0 / translateX(50px) to rest over 1s cubic-bezier(.34,1.56,.64,1), 20ms apart; the plain heading is restored on the last `animationend`.
- **Fade-up:** elements that start below the first screen rise 12px and fade in over 0.4s ease-out once; anything visible at load is never hidden.
- **Reduced motion:** all of the above, smooth scroll and button transitions are switched off.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed paper and navy bands, putting the line texture only on the deep navy (and the no-photo hero).
- **Do** use Sparkle Gold as a fill with Ink text, and Gold Ink whenever gold has to be text on paper.
- **Do** set headings, buttons, labels and list rows in Cal Sans 400 and everything else in the system stack at 16px / 1.7.
- **Do** keep shapes soft and borderless: 24px cards, 10px fields on the Field tint, full pills, 44px+ tap targets.
- **Do** route every new contact point through `data-reach` and `CONFIG` so the phone switch reaches it.
- **Do** gate hover styles behind `(hover:hover)` and honour `prefers-reduced-motion`.
- **Do** put a client photo behind the hero under a navy overlay if one later becomes available and fits both phone and desktop shapes.

### Don't:
- **Don't** put white text on gold or gold text on paper; both fail contrast.
- **Don't** add shadows to cards, buttons or chips; only the floating circle lifts.
- **Don't** add a second accent colour, a second display face or bold display weights.
- **Don't** apply the bounce-in to any heading other than the hero H1, or fade in anything already on the first screen.
- **Don't** turn the floating circle into a bottom bar or show it over the form.
- **Don't** add eyebrow pills beyond the two the build carries (see note below); they are an owner-approved exception, not a pattern to extend.
- **Don't** invent photos, logos, reviews, prices or badges to fill space.

**Carried exception, not a system rule.** The build has two eyebrow pills (hero "Now accepting new clients", estimate "Free, no obligation"): 14px system text on a 6% ink (12% white on navy) pill with a gold dot. They are the owner's chosen calm-style exception and conflict with Impeccable's craft floor; they are recorded here as present in the build only, and new surfaces should not inherit them.
