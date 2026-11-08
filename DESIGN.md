---
name: Acid Paper Editorial
colors:
  surface: '#fcf8fb'
  surface-dim: '#dcd9dc'
  surface-bright: '#fcf8fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f2f5'
  surface-container: '#f0edf0'
  surface-container-high: '#eae7ea'
  surface-container-highest: '#e5e1e4'
  on-surface: '#1c1b1d'
  on-surface-variant: '#464833'
  inverse-surface: '#313032'
  inverse-on-surface: '#f3f0f2'
  outline: '#777961'
  outline-variant: '#c7c8ad'
  surface-tint: '#596400'
  primary: '#596400'
  on-primary: '#ffffff'
  primary-container: '#d2e823'
  on-primary-container: '#5b6600'
  inverse-primary: '#bdd200'
  secondary: '#1d4ed8'
  on-secondary: '#ffffff'
  secondary-container: '#4069f2'
  on-secondary-container: '#fffbff'
  tertiary: '#be0037'
  on-tertiary: '#ffffff'
  tertiary-container: '#ffd1d2'
  on-tertiary-container: '#c20038'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d8ef2c'
  primary-fixed-dim: '#bdd200'
  on-primary-fixed: '#1a1e00'
  on-primary-fixed-variant: '#434b00'
  secondary-fixed: '#dce1ff'
  secondary-fixed-dim: '#b7c4ff'
  on-secondary-fixed: '#001551'
  on-secondary-fixed-variant: '#0039b5'
  tertiary-fixed: '#ffdada'
  tertiary-fixed-dim: '#ffb3b6'
  on-tertiary-fixed: '#40000c'
  on-tertiary-fixed-variant: '#920028'
  background: '#fcf8fb'
  on-background: '#1c1b1d'
  surface-variant: '#e5e1e4'
typography:
  display-xl:
    fontFamily: Onest
    fontSize: 72px
    fontWeight: '700'
    lineHeight: 76px
    letterSpacing: -0.04em
  display-xl-mobile:
    fontFamily: Onest
    fontSize: 44px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Onest
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.03em
  headline-lg-mobile:
    fontFamily: Onest
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Onest
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Onest
    fontSize: 20px
    fontWeight: '700'
    lineHeight: 24px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Onest
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 26px
    letterSpacing: -0.01em
  body-md:
    fontFamily: Onest
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 22px
    letterSpacing: 0em
  body-sm:
    fontFamily: Onest
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
    letterSpacing: 0em
  label-lg:
    fontFamily: Onest
    fontSize: 14px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.06em
  label-md:
    fontFamily: Onest
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 14px
    letterSpacing: 0.08em
  label-sm:
    fontFamily: Onest
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 12px
    letterSpacing: 0.1em
spacing:
  gutter: 1.5rem
  gutter-mobile: 0.75rem
  margin: 2.5rem
  margin-mobile: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2.5rem
---

## Brand & Style

This design system blends uncompromising neo-brutalist structure with razor-sharp editorial magazine art direction. Designed for an intellectual, avant-garde psychological game club, the atmosphere balances raw mechanical clarity with high-voltage visual tension. 

Key attributes:
- **Intellectually Confrontational:** Dense, typographic layouts that demand focus rather than passive consumption.
- **Physical Print Artifact:** Rooted in pulpy broadsheets, technical manifestos, and underground gaming publications.
- **Hard-Edged Tactility:** Solid, unblurred drop shadows and stark high-contrast borders provide physical snap and mechanical feedback.
- **Kinetic Energy:** The collision of warm, natural newsprint tones with synthetic, hyper-saturated acid accents generates relentless optical vibration.

## Colors

The palette relies on absolute contrast and deliberate chemical friction.

- **Paper Canvas (`#F8F4E8`):** The primary surface foundation. An unbleached, high-density pulp milk tone that prevents digital glare while grounding saturated pigments.
- **Ink Black (`#09090B`):** Deep, impenetrable structural ink. Used for structural grid strokes, heavy typographic blocks, and mechanical 0-blur shadows.
- **Acid Yellow-Green (`#D2E823`):** The primary energy catalyst. Reserved for active states, critical calls to action, priority badges, and highlighted editorial copy.
- **Cobalt Blue (`#1D4ED8`):** Deep cerebral blue. Serves as a rational counterweight for systems status, deep links, structural accents, and secondary actions.
- **Tomato Red (`#E11D48`):** Urgent, visceral editorial signal. Dictates warnings, high-stakes game parameters, countdowns, and destructive triggers.
- **Surface Variant (`#ECE7D5`):** A shaded newsprint tier used for secondary card backing and input well fills without breaking the physical paper feel.

## Typography

The typography is built around high-density mechanical forms. Onest is deployed across all levels, utilizing heavy weight variations, negative tracking at large scales, and uppercase tracking for metadata.

- **Display & Headlines:** Set in bold weights with tight leading (`0.95` to `1.1`) and negative tracking. Headings should be punctuated aggressively, frequently utilizing full capitalization for key editorial phrases.
- **Body Text:** Balanced at medium weights for dense editorial blocks. Never thin or light. Maintain a strict 65–75 character measure to preserve the broadsheet reading cadence.
- **Metadata & Labels:** Always rendered in uppercase with wide letter-spacing (`0.06em` to `0.1em`) to mimic stamped manifestos, dossier headers, and tactical readouts.

## Layout & Spacing

The layout philosophy mirrors an asymmetric, broadsheet magazine grid. Content does not conform to soft centered containers; instead, it is pinned directly against mechanical gutters and structural rules.

- **Grid Architecture:** 12-column desktop fluid layout breaking into an asymmetrical 8-column tablet and 4-column mobile structure. Elements snap into uneven spans (e.g., a 7-column primary narrative alongside a 5-column dossier card).
- **Hard Boundaries:** Visual partitions are enforced through physical 2px and 4px solid `#09090B` rules rather than soft white space.
- **Rhythm:** Spacing tokens operate on strict multiples of 4px/8px. Component internal padding favors compact, horizontal tension (`space-sm` vertical by `space-lg` horizontal) to reinforce horizontal striping and ticket-stub visual metaphors.

## Elevation & Depth

This system discards Gaussian blurs, soft drop-shadows, and faux lighting entirely. Depth is structural, mechanical, and binary.

- **0-Blur Hard Shadows:** Elevation is achieved solely via hard-offset solid black drop shadows:
  - **Flat / Grounded:** `0px 0px 0px #09090B` (standard surface level).
  - **Raised (Cards, Interactive Modules):** `4px 4px 0px 0px #09090B`.
  - **Floating (Modals, Overlays, Floating Action Banners):** `8px 8px 0px 0px #09090B`.
  - **Active / Pressed:** `0px 0px 0px 0px #09090B` with an immediate translate offset (`translate(4px, 4px)` or `translate(2px, 2px)`).
- **Structural Outlines:** Every card, container, button, and divider possesses a mandatory `2px` or `4px` solid `#09090B` border.
- **Stacking Logic:** Elements do not blend; they occlude. Overlapping cards produce rigid paper cutout silhouettes with zero transparency.

## Shapes

The shape vocabulary is strictly non-filleted:
- **Zero Radius:** All corners remain `0px`. Sharp, unsoftened edges throughout.
- **Angle Variations:** Angled corner notches (45-degree chamfers measuring 8px to 12px) may be applied to badges, document headers, and game tokens to emulate punch cards and cut ticket stock.
- **Dividers & Strokes:** Linear elements must be sharp-ended vectors with square caps (`stroke-linecap: square`).

## Components

### Buttons
- **Primary:** Background `#D2E823`, text `#09090B`, border `3px solid #09090B`, shadow `4px 4px 0px #09090B`. On hover: shadow expands to `6px 6px 0px #09090B`, slight negative translation. On active: translate `4px 4px`, shadow `0px 0px 0px`.
- **Secondary:** Background `#F8F4E8`, text `#09090B`, border `2px solid #09090B`, shadow `3px 3px 0px #09090B`. Hover flips background to `#1D4ED8` and text to `#F8F4E8`.
- **Destructive:** Background `#E11D48`, text `#F8F4E8`, border `3px solid #09090B`, shadow `4px 4px 0px #09090B`.

### Badges & Tags
- Set in `label-sm` or `label-md` uppercase Onest.
- Border `2px solid #09090B`. Padding `2px 8px`.
- Status variants: Acid (`#D2E823`), Cobalt (`#1D4ED8` with `#F8F4E8` text), Crimson (`#E11D48` with `#F8F4E8` text), or Raw Paper (`#ECE7D5`).
- Optional hard shadow: `2px 2px 0px #09090B`.

### Cards & Dossiers
- Background `#F8F4E8` or `#ECE7D5`.
- Border `3px solid #09090B`, shadow `4px 4px 0px #09090B`.
- Header zone separated by a solid `2px` horizontal border.
- Interactive cards translate into their shadow upon click (`translate(2px, 2px)` with shadow reduced to `2px 2px 0px`).

### Input Fields
- Background `#F8F4E8`, border `2px solid #09090B`, padding `12px 16px`.
- Focus state: Outline remains crisp, border thickens to `3px solid #09090B`, accompanied by an instant hard shadow `4px 4px 0px #D2E823`.
- Placeholder text in `#09090B` with `50%` opacity.

### Checkboxes & Radio Buttons
- Square geometry (`roundedness: 0`), `20px x 20px`, border `2px solid #09090B`, shadow `2px 2px 0px #09090B`.
- Checked state: Background `#D2E823`, filled with a stark black interior square (checkbox) or centered solid block (radio).

### Lists & Tables
- Divided strictly by `2px solid #09090B` horizontal rules.
- Table headers set in solid `#09090B` with high-contrast `#F8F4E8` text.
- Alternate rows or hover states trigger `#D2E823` or `#ECE7D5` full-width highlight bars.

### Club Tactical Components
- **Index Counters:** Oversized numeral counters set in bold headline scales accompanied by a `2px solid #09090B` bounding box.
- **Redaction Bars:** Blackout bars (`background: #09090B`) masking text blocks, revealing contents with an Acid yellow highlight on hover.