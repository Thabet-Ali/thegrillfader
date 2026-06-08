---
name: The Grillfader
description: Fire-built BBQ catering by one pitmaster — a cinematic, single-page invitation.
colors:
  oxblood: "#5E1414"
  oxblood-seared: "#7A1C1C"
  aged-brass: "#B08D57"
  ember: "#E8772E"
  char-black: "#120D0C"
  banked-coal: "#1B1411"
  calendar-pit: "#15110D"
  candlelight-cream: "#EDE6D8"
  warm-ash: "#D6CDBC"
  smoke: "#8A8780"
typography:
  wordmark:
    fontFamily: "UnifrakturCook, Cinzel, serif"
    fontWeight: 700
    purpose: "Blackletter logotype only."
  display:
    fontFamily: "Cinzel, Georgia, serif"
    fontSize: "clamp(2.7rem, 1.7rem + 4.6vw, 5.4rem)"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.005em"
  statement:
    fontFamily: "Cinzel, Georgia, serif"
    fontSize: "clamp(2.1rem, 1.4rem + 3.4vw, 4.2rem)"
    fontWeight: 700
    lineHeight: 1.06
  body:
    fontFamily: "Jost, system-ui, -apple-system, sans-serif"
    fontSize: "1rem"
    fontWeight: 300
    lineHeight: 1.65
  lede:
    fontFamily: "Jost, system-ui, sans-serif"
    fontSize: "clamp(1.15rem, 1.02rem + 0.6vw, 1.5rem)"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Jost, system-ui, sans-serif"
    fontSize: "clamp(0.85rem, 0.75rem + 0.4vw, 1.05rem)"
    fontWeight: 600
    letterSpacing: "0.38em"
    textTransform: "uppercase"
rounded:
  hairline: "2px"
  sm: "4px"
  control: "7px"
  panel: "10px"
  card: "16px"
  pill: "100px"
spacing:
  gut: "clamp(1.25rem, 5vw, 4rem)"
  maxw: "1180px"
components:
  button-primary:
    backgroundColor: "{colors.oxblood}"
    textColor: "{colors.candlelight-cream}"
    typography: "{typography.display}"
    rounded: "{rounded.sm}"
    padding: "1.1rem 2rem"
  button-primary-hover:
    backgroundColor: "{colors.oxblood-seared}"
    textColor: "{colors.candlelight-cream}"
  button-nav-cta:
    backgroundColor: "transparent"
    textColor: "{colors.aged-brass}"
    rounded: "{rounded.hairline}"
    padding: "0.55rem 1.15rem"
  button-nav-cta-hover:
    backgroundColor: "{colors.aged-brass}"
    textColor: "{colors.char-black}"
  input-field:
    backgroundColor: "transparent"
    textColor: "{colors.candlelight-cream}"
    padding: "0.7rem 0"
  chip-stepper:
    backgroundColor: "transparent"
    textColor: "{colors.warm-ash}"
    rounded: "{rounded.pill}"
    padding: "0.5rem 0.9rem"
---

# Design System: The Grillfader

## 1. Overview

**Creative North Star: "The Opening Scene"**

This is the hush before a film begins. The room is dark, a single flame is the only
light, and one figure stands in it who clearly knows exactly what he is doing. Every
screen of The Grillfader holds that frame: near-black ground, fire as the source of
warmth and motion, type cut from stone, and copy spoken in the first person by a man who
answers to no one. The site is a single-page invitation, not a brochure. It opens on a
flame-lit logo, walks you through an origin and a menu, and arrives at one quiet
proposition: book him.

Restraint is the luxury signal here, never ornament. Warmth is carried by ember glow,
aged brass, and the human voice, never by softness, friendliness, or a warm-tinted body
background. Imagery does the heavy lifting (full-bleed fire, food shot like portraits,
Ken Burns drift on everything), and the chrome recedes so the photograph and the
headline can carry the fold. When a section feels busy, the fix is to remove an element
and enlarge what stays.

This system explicitly rejects the generic catering/restaurant template (stock-photo
grids, "welcome to our restaurant", smiling-staff heroes), the rustic-farmhouse BBQ
joint (chalkboard fonts, kraft paper, distressed wood, mason jars), and the loud
SaaS/startup landing (gradient blobs, glassmorphism, eyebrow kickers over every section,
identical feature-card grids). It is luxury and cinematic, not down-home and not
template.

**Key Characteristics:**
- Near-black, fire-lit ground; ember and brass are the only warmth.
- Cinzel cut-stone display against Jost light body; UnifrakturCook reserved for the logo.
- Full-bleed imagery with perpetual Ken Burns drift; chrome recedes to let it lead.
- Forged, deliberate controls: oxblood blocks, ember-glow on commit, hairline brass borders.
- One idea per fold; long, paced scroll that ends at the booking.

## 2. Colors

A fire-lit darkroom: a near-black ground lit by a single fire, with oxblood for
authority and brass for the gilded edges. Color is Committed, not restrained, but the
saturation lives in fire and blood, never in a tinted neutral.

### Primary
- **Oxblood** (`#5E1414`): The brand's blood. Carries the primary action (the booking
  submit), text selection, and any moment that must read as decisive. Deep, dried-blood
  red, never bright or cherry.
- **Seared Oxblood** (`#7A1C1C`): The hover/active deepening of Oxblood. Used only as the
  pressed state of the primary button; never as a resting fill.

### Secondary
- **Ember** (`#E8772E`): Fire made into an accent. The focus color on every field, the
  selected calendar day, the live guest count, the glow under the submit on hover, and
  the scroll-progress bar. Ember means "this is alive / this is active." Use it sparingly;
  its rarity is what makes it read as heat.

### Tertiary
- **Aged Brass** (`#B08D57`): The gilded edge. Eyebrow/kicker labels, hairline borders on
  cards and inputs, social-icon strokes, the shimmering gold dividers between dishes, nav
  link underlines. The constant "fine establishment" signal threaded through the chrome.

### Neutral
- **Char Black** (`#120D0C`): The body ground. Warm-leaning near-black; the darkroom the
  whole site lives in.
- **Banked Coal** (`#1B1411`): The one raised surface (the offer/booking panel). A single
  step up from the ground, no boxy card stack.
- **Calendar Pit** (`#15110D`): The deepest popover ground (the date picker), reading as a
  recess below the page.
- **Candlelight Cream** (`#EDE6D8`): Primary text and the logo fill. Warm off-white that
  reads as light thrown by flame, not paper.
- **Warm Ash** (`#D6CDBC`): Secondary/lede body text and chip labels; a step down from
  cream for supporting copy.
- **Smoke** (`#8A8780`): Muted metadata, stat labels, calendar day-of-week headers. The
  quietest readable tone; never used for primary body copy.

### Named Rules
**The Fire-Lit Rule.** The ground is always dark and warm-leaning; never a tinted near-white
"cream" background. "Cream" in this system is a *text* color thrown by candlelight, not a
surface. A light body background breaks the opening-scene frame entirely.

**The Ember-Is-Alive Rule.** Ember (`#E8772E`) marks only live or active state: focus,
selection, the current count, a hover glow. It is never a decorative fill or a resting
color. If something is ember and isn't reacting to the user, it's wrong.

## 3. Typography

**Wordmark Font:** UnifrakturCook (with Cinzel, serif fallback) — logotype only.
**Display Font:** Cinzel (with Georgia, serif)
**Body Font:** Jost (with system-ui, -apple-system, sans-serif)

**Character:** Cinzel is Roman inscription cut into stone: authority, permanence, the
name on the building. Jost is a clean geometric sans set very light (300), which keeps the
body quiet so the stone headlines and the fire imagery carry the weight. The contrast axis
is engraved-serif against light-geometric-sans, a deliberate, wide pairing. UnifrakturCook
(blackletter) appears once, as the logo, where it reads as crest and old-world authority;
it is forbidden anywhere in running text.

### Hierarchy
- **Wordmark** (UnifrakturCook 700): The Grillfader logotype only. Never body, never headings.
- **Display** (Cinzel 700, `clamp(2.7rem → 5.4rem)`, line-height 1, +0.005em): Section
  titles. Cut-stone headlines that open each fold.
- **Statement** (Cinzel 700, `clamp(2.1rem → 4.2rem)`, line-height 1.06): The first-person
  declarations ("I don't cater parties. I run them."). The pitmaster's voice in stone.
- **Lede** (Jost 400, `clamp(1.15rem → 1.5rem)`, line-height 1.6, Warm Ash): The intro
  paragraph under a heading. Capped at ~54ch.
- **Body** (Jost 300, 1rem, line-height 1.65, Candlelight Cream): Running copy. Light
  weight; on the dark ground the generous 1.65 leading keeps the thin strokes legible.
- **Label** (Jost 600, `clamp(0.85rem → 1.05rem)`, +0.38em tracking, uppercase, Aged
  Brass): The kicker/eyebrow and field labels. The one place uppercase tracking is allowed.

### Named Rules
**The Stone-and-Smoke Rule.** Cinzel is for things carved to last (names, headings,
declarations, numbers). Jost is for things spoken aloud (running copy, lede, labels). Never
set body copy in Cinzel or a heading in Jost.

**The Light-Body Rule.** Body is Jost 300 on a dark ground, so line-height never drops
below 1.6. Thin light type on black needs the air; tightening it makes the page hard to read.

## 4. Elevation

This system is shadow-light and depth-rich. There are no boxy, layered card stacks. Depth
comes from three things: tonal layering (Char Black ground → Banked Coal panel → Calendar
Pit recess), warm fire glow rather than gray drop shadows, and full-bleed imagery with
gradient grades. Shadows, when used, are deep, near-black, and long, reading as the dark
swallowing an edge, plus ember-colored glows that read as heat, not as a floating UI layer.

### Shadow Vocabulary
- **Panel sink** (`box-shadow: 0 44px 120px -44px rgba(0,0,0,.92)`): The offer/booking
  panel settling into the dark. A single deep, soft, near-black shadow; the surface sits
  *in* the room, not floating above it.
- **Popover lift** (`box-shadow: 0 28px 70px -22px rgba(0,0,0,.85)`): The calendar
  popover. Deep black, never gray.
- **Ember commit glow** (`box-shadow: 0 18px 55px -14px rgba(232,119,46,.6)`): The booking
  submit on hover. Heat thrown forward, the only colored shadow in the system.
- **Brass hairline glow** (`box-shadow: 0 0 10px rgba(176,141,87,.55)`): Under the gold
  dividers; a faint gilded shimmer, not elevation.

### Named Rules
**The No-Gray-Shadow Rule.** Shadows are near-black (`rgba(0,0,0,...)`) or fire-colored
(ember/brass glow). A neutral gray shadow reads as generic UI chrome and breaks the
darkroom. Depth on this page is the dark swallowing edges, not panels floating on white.

## 5. Components

Controls are **forged and deliberate**: heavy where they commit, hairline where they
support, fire-touched when they react. Nothing tentative, nothing bouncy.

### Buttons
- **Shape:** Crisp, near-square. Primary at 4px (`{rounded.sm}`), nav CTA at 2px
  (`{rounded.hairline}`). No pill-shaped primary buttons; pills are reserved for chips/tags.
- **Primary (booking submit):** Solid Oxblood block, Candlelight Cream label set in Cinzel
  700 uppercase (+0.12em), full-width, padding `1.1rem 2rem`. The one heavy, committed
  element on the page.
- **Hover / Focus:** Background deepens to Seared Oxblood, lifts `translateY(-2px)`, and
  throws the Ember commit glow. Reads as the fire flaring when you commit.
- **Nav CTA:** Brass hairline outline, brass text, transparent fill; inverts to a solid
  brass fill with Char Black text on hover. Quiet until you reach for it.

### Chips & Steppers
- **Style:** Pill (`{rounded.pill}`), transparent fill, brass hairline border, Warm Ash
  label, uppercase tracked. Used for the guest-count presets.
- **State:** Hover fills to faint brass (`rgba(176,141,87,.14)`), border brightens to full
  brass, text to cream. The live guest number itself is large Cinzel in Ember (it is alive).

### Cards (the catering accordion)
- **This is the signature component; it is NOT a static card grid.** Four full-height
  image tiles sit in a flex row. On hover the row contracts every tile (`flex-grow: .88`)
  and expands the hovered one (`flex-grow: 1.55`) over 0.6s, revealing its description and
  an "explore" pill. Each tile runs a perpetual Ken Burns drift (one diagonal per tile,
  12s).
- **Corner Style:** 18px on the tiles (softer than the rest of the system, because the
  image needs the rounding).
- **Grade:** A top-and-bottom darkening gradient for legibility, never a flat scrim.
- **Mobile:** The accordion collapses to clean stacked photos; tag + title pinned at the
  bottom, the whole card taps through to booking. No hover-only content on touch.

### Inputs / Fields
- **Style:** Editorial underline only. Transparent fill, no box; a 1.5px Aged Brass bottom
  border, Jost body text at 1.18rem, placeholder at warm-ash 38% opacity. `border-radius: 0`.
- **Focus:** Bottom border shifts to Ember. No box glow, no fill change; the line catches fire.
- **Labels:** Brass, uppercase, +0.2em tracked, above the field.

### Custom Date Picker & Stepper
- **Calendar:** Opens into Calendar Pit (`#15110D`) with a brass hairline border and the
  Popover lift shadow. Selected day fills Ember with dark text; today/hover fills faint brass.
- **Guests stepper:** Square 54px brass-hairline +/- buttons flanking a huge Ember Cinzel
  count, with a tier caption and preset pills below.

### Navigation
- **Style:** Fixed, transparent over the hero; on scroll it fills to `rgba(18,13,12,.72)`
  with a 14px backdrop blur and a brass hairline bottom border.
- **Links:** Jost, uppercase, +0.16em tracked, warm gray, with a brass underline that grows
  from 0 to 100% width on hover. The cinematic equivalent of a quiet menu.
- **Mobile:** Collapses to a minimal menu; nav choices clamp down so they never wrap.

### Signature Flourishes
- **Shimmering gold dividers** between dishes: a layered metallic gradient with a moving
  highlight (`goldshine` 3.4s) under a mask, plus the brass hairline glow. Reads as real gilt.
- **Scroll-progress bar:** A 2px brass→ember gradient line, fixed at the top, with an ember glow.

## 6. Do's and Don'ts

### Do:
- **Do** keep the ground Char Black (`#120D0C`) or its tonal siblings. Warmth comes from
  ember, brass, and fire imagery, never from the background.
- **Do** reserve Ember (`#E8772E`) for live/active state only (focus, selection, current
  count, commit glow). Its rarity is the heat.
- **Do** set every heading and declaration in Cinzel, every line of running copy in Jost
  300 with line-height ≥ 1.6.
- **Do** lead with full-bleed imagery and let Ken Burns drift carry the motion; let the
  photograph be the design.
- **Do** use deep near-black or fire-colored shadows for depth; layer tonally (ground →
  panel → recess).
- **Do** point every fold at the booking, and when a section feels busy, remove an element
  and enlarge what remains.

### Don't:
- **Don't** introduce a cream/sand/beige *background*. "Cream" is a text color here. A
  light body bg breaks the opening-scene frame.
- **Don't** drift into the **generic catering/restaurant template**: stock-photo grids,
  "welcome to our restaurant", smiling-staff heroes.
- **Don't** go **rustic-farmhouse BBQ**: chalkboard fonts, kraft paper, distressed wood,
  mason jars, "smokehouse" clichés. This is luxury.
- **Don't** import the **loud SaaS/startup landing**: gradient blobs, glassmorphism as
  decoration, tiny tracked eyebrows over *every* section, hero-metric templates, identical
  feature-card grids.
- **Don't** clutter or over-decorate. Nothing may fight the cinematic restraint; one idea
  per fold.
- **Don't** use gray drop shadows, pill-shaped primary buttons, side-stripe accent borders,
  or gradient text. Depth is the dark swallowing edges, not floating panels.
- **Don't** set UnifrakturCook anywhere but the logo, or body copy in Cinzel.
