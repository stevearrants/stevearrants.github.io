---
name: Green Mountain Docs
description: Technical writing consultancy for Steve Arrants — expert, precise, direct.
colors:
  summit-green-dark: "#2D6A4F"
  summit-green: "#27AE60"
  alpine-slate: "#2C3E50"
  alert-blue: "#2980B9"
  link-blue: "#1A6FA8"
  fog-grey: "#ECF0F1"
  white: "#FFFFFF"
  footer-dark: "#162923"
  footer-link-green: "#6DBF96"
typography:
  display:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, sans-serif"
    fontSize: "clamp(1.75rem, 4vw, 2.75rem)"
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, sans-serif"
    fontSize: "clamp(1.35rem, 2.5vw, 1.75rem)"
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Merriweather, Georgia, serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.7
    letterSpacing: "normal"
  label:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: "0.01em"
rounded:
  sm: "3px"
  md: "4px"
  lg: "8px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "48px"
components:
  button-primary:
    backgroundColor: "{colors.summit-green-dark}"
    textColor: "{colors.white}"
    rounded: "{rounded.md}"
    padding: "12px 24px"
  button-primary-hover:
    backgroundColor: "#1A5C3A"
    textColor: "{colors.white}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.summit-green-dark}"
    rounded: "{rounded.md}"
    padding: "10px 22px"
  tag-chip:
    backgroundColor: "{colors.summit-green}"
    textColor: "{colors.white}"
    rounded: "{rounded.sm}"
    padding: "4px 8px"
---

# Design System: Green Mountain Docs

## 1. Overview

**Creative North Star: "The Senior Advisor's Office"**

Green Mountain Docs presents as a senior practitioner's workspace: functional, uncluttered, and quietly confident. Nothing decorates; everything informs. The visual system earns trust through clarity, not through polish — a potential client should feel they're being assessed by the same rigorous standard Steve applies to their documentation.

The palette carries weight without drama: a deep forest green that reads as deliberate (not corporate), a dark slate for text that commands without shouting, and a light neutral ground that recedes so the content can advance. Links are a restrained blue — functional, not playful. The only flash of brightness is reserved for secondary interactive states, where it acts as a brief acknowledgment rather than an accent.

This is a system built for a writer. Typography is the primary expressive tool. Merriweather body text signals that the author takes reading seriously; Inter headings signal precision. Motion and decoration are minimal; when the prose is the portfolio, the design gets out of the way.

**What this system explicitly rejects:** Generic freelancer templates (Upwork-style layout, soft-focus hero photography, skill-pill grids, "hire me" cadence). Startup/SaaS marketing moves: gradient blobs, hero metrics, glassmorphism, feature cards with icons over every bullet.

**Key Characteristics:**
- High-contrast type on neutral ground — readability first
- Forest green as the single committed accent, used sparingly
- Merriweather body for long-form credibility; Inter headlines for directness
- Flat surfaces with minimal shadow — depth through typography, not decoration
- Direct copy, no hedging, no adjective inflation

## 2. Colors: The Mountain Workspace Palette

A five-color working palette anchored by deep forest green and dark slate, supported by a light neutral ground. No gradients, no mixing.

### Primary
- **Forest Anchor** (#2D6A4F): The primary action color. CTAs, navbar border accent, hover-active links, tag badges in hover state. Used sparingly — its restraint gives it weight.
- **Summit Green** (#27AE60): Lighter accent variant. Tag/chip backgrounds, date labels, timeline dots. Never used on text over white (contrast insufficient).

### Secondary
- **Link Blue** (#1A6FA8): Hyperlinks in body text. Distinguishable from the green accent without competing.
- **Alert Blue** (#2980B9): Hover state for links; secondary CTA hover; tag hover backgrounds. A brief, functional response state.

### Neutral
- **Alpine Slate** (#2C3E50): Primary text color. Footer background. The heaviest neutral — authoritative, not black.
- **Fog Grey** (#ECF0F1): Page background. Gives the canvas a hair of warmth compared to pure white without reading as cream. Direction: nudge slightly warmer in future iterations (`#F2F4EE` or equivalent cool-to-neutral tint at the brand's own hue).
- **White** (#FFFFFF): Card/surface backgrounds, navbar. Pure white against the grey page creates clean surface separation.
- **Footer Dark** (#162923): Footer background — a very dark forest green. Ties footer to the primary palette without reusing the active accent.
- **Footer Link Green** (#6DBF96): Links and link hover in the footer context, where contrast against the dark background is the priority.

### Named Rules
**The One Accent Rule.** Summit green (#2D6A4F) appears on interactive elements and key structural moments only. It does not appear as a decorative stripe, background wash, or repeated divider. Its rarity carries the brand voice; dilution erases it.

## 3. Typography

**Display/Heading Font:** Inter (with -apple-system, BlinkMacSystemFont, sans-serif fallback)
**Body Font:** Merriweather (with Georgia, serif fallback)

**Character:** Inter's geometric precision reads as "engineer adjacent" — appropriate for a consultant who works in CLI, Git, and structured content platforms. Merriweather's small-x-height serif signals that the author takes long-form reading seriously. The contrast between the two is the voice: systems thinking, fluent writing.

*Note for future redesigns:* Inter appears on the brand register's reflex-reject list due to saturation. If the site undergoes a significant redesign, consider a less ubiquitous geometric sans for headings — Aktiv Grotesk, Neue Haas Grotesk, or ABC Diatype carry the same "precise without being cold" register with more distinctiveness.

### Hierarchy
- **Display** (700, clamp(1.75rem → 2.75rem), lh 1.15, ls -0.02em): Page-level titles, hero headings. Used once per page.
- **Headline** (700, clamp(1.35rem → 1.75rem), lh 1.25, ls -0.01em): Section headings, service names. Sets the structural scan path.
- **Title** (600, 1.125rem, lh 1.35): Subsection labels, card titles, list item heads.
- **Body** (400, 1rem / 16px, lh 1.7, Merriweather): All prose. Max line length 65–75ch. Merriweather at 1.7 line-height reads comfortably at this weight.
- **Label** (Inter, 600, 0.875rem, ls 0.01em): Tags, dates, metadata, button text, navigation items.

### Named Rules
**The Serif Body Rule.** Merriweather is the only serif in the system. Body text is always serif. Headings, labels, and UI copy are always Inter (or its replacement). Mixing serif into headings — or pulling sans into body prose — breaks the contract.

## 4. Elevation

This system is flat by default. Depth is conveyed through background contrast (white cards on grey page) and border treatment, not through shadow stacking. Shadows exist as functional signals: the appearance of a shadow means something has lifted in response to user action.

### Shadow Vocabulary
- **Ambient-low** (`0 2px 4px rgba(0,0,0,0.10)`): Resting card elevation. Portfolio items, content blocks at rest.
- **Ambient-medium** (`0 2px 8px rgba(0,0,0,0.05)`): Lighter structural containers. Use when a surface needs to separate from the page without announcing itself.
- **Hover-lift** (`0 4px 12px rgba(0,0,0,0.15)`): Interactive surfaces on hover. Confirms that an element is actionable.

### Named Rules
**The Flat-By-Default Rule.** Surfaces are flat at rest. Shadows appear only as a state response (hover, active elevation). A static element with a large box-shadow is a design error, not a style choice.

## 5. Components

### Buttons
- **Shape:** Gently rounded (4px radius). Not pill-shaped; not sharp-cornered.
- **Primary:** Forest Anchor (#2D6A4F) background, white text, 12px 24px padding. Font: Inter 600. Full-width on mobile, inline on desktop.
- **Hover:** Darkens to #1A5C3A, 2px vertical lift (`translateY(-2px)`), hover-lift shadow.
- **Ghost / Outline:** Transparent background, 2px Forest Anchor border, Forest Anchor text. Peer button to primary; used when two CTAs appear together.
- **Transition:** `background-color 0.25s ease, transform 0.2s ease, box-shadow 0.2s ease`.

### Chips / Tags
- **Style:** Summit Green (#27AE60) background, white text, 3px radius, 4px 8px padding.
- **Hover:** Alert Blue (#2980B9) background.
- **Size:** Label scale (Inter 600, 0.85rem). Single-line only.

### Cards / Containers
- **Corner Style:** Gently rounded (8px radius) for structural containers; 4px for inline content blocks.
- **Background:** White (#FFFFFF) against Fog Grey page.
- **Shadow:** Ambient-low at rest (`0 2px 4px rgba(0,0,0,0.10)`).
- **Border:** None as default. The white-on-grey contrast is sufficient separation. Exception: timeline items use a 2px left border as a structural guide (not a decorative stripe).
- **Internal Padding:** 24px (`spacing.lg`).

### Inputs / Fields
- **Style:** 1px solid border (#DDDDDD at rest), white background, 4px radius.
- **Focus:** Border shifts to Forest Anchor (#2D6A4F). No glow; the border shift is the signal.
- **Placeholder:** Must meet 4.5:1 against white background. Do not use the browser default light grey.

### Navigation
- **Style:** White background, 2px Forest Anchor bottom border. Text: Alpine Slate, Inter 600. No decorative elements.
- **Active/Hover:** Link text shifts to Forest Anchor.
- **Mobile:** Collapses to hamburger. Theme-consistent colors throughout.

### Post Previews (Blog)
- **Structure:** Merriweather title, truncated Merriweather excerpt, Inter label metadata (date, tags).
- **Separation:** Margin-based spacing between items. No border-left stripe — use whitespace as the separator.

## 6. Do's and Don'ts

### Do:
- **Do** use Forest Anchor (#2D6A4F) for the primary CTA and key structural accents only. Reserve it for elements that need to command attention.
- **Do** set body text in Merriweather at 1.7 line-height, capped at 65–75ch per line.
- **Do** use white cards on a Fog Grey page for surface separation — no border needed when contrast is doing the work.
- **Do** apply hover-lift shadow (`0 4px 12px rgba(0,0,0,0.15)`) to interactive surfaces on hover so affordance is visible.
- **Do** use `text-wrap: balance` on h1–h3 to prevent orphaned words at narrow widths.
- **Do** verify body text contrast at ≥ 4.5:1 against the page background, including placeholder text in inputs.

### Don't:
- **Don't** use `border-left` wider than 1px as a colored accent stripe on cards, post previews, or list items. This includes the existing `.post-preview { border-left: 4px }` and `.portfolio-item { border-left: 4px }` patterns — replace with margin-based spacing or background tint.
- **Don't** produce a generic freelancer template aesthetic: Upwork-style skill-pill grids, soft-focus hero photography, "hire me" sentence cadence, bullet-point capability lists without specificity.
- **Don't** use startup/SaaS marketing moves on this surface: gradient text (`background-clip: text`), hero metrics (big number + small label), glassmorphism, feature-card icon grids.
- **Don't** add icon-above-heading layout for every service or section. If an icon appears, it should serve information, not decoration.
- **Don't** apply the same reveal animation to every section as section scaffolding. Motion is purposeful or absent.
- **Don't** use `border-left: 4px` as a visual shorthand for "important" — this pattern appears in `.post-preview`, `.portfolio-item`, `.service-item`, and `.timeline-item` across the current codebase and should be audited and replaced.
- **Don't** dilute the Forest Anchor green by spreading it across dividers, backgrounds, or decorative borders. Rarity is the mechanism.
