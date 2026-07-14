---
version: alpha
name: Zilliz Brand
description: The official Zilliz design system — a deep near-black canvas carrying the signature Zilliz brand gradient (sky blue → blue → purple → berry) as the single expressive device, with electric Zilliz Blue (#175FFF) as the solid accent. Inter runs every headline and body line; IBM Plex Mono handles eyebrows, labels, metrics, and technical chrome to signal the vector-database register. Hero words use gradient-clipped text; surfaces are lifted with subtle translucent cards rather than shadows; decoration is built from abstract "vector coordinate" diagonal lines and thin gradient arcs — never a recreated Zilliz logo. The aesthetic is modern, technical, confident, and unmistakably Zilliz: dark, luminous, and gradient-forward.

colors:
  bg: "#000000"
  bg-elevated: "#0C0E16"
  navy: "#061982"
  primary: "#175FFF"
  sky: "#49BCFF"
  purple: "#7F47FF"
  berry: "#C84CFF"
  green: "#00DCC6"
  text: "#FFFFFF"
  text-muted: "#A9B0C0"
  text-light: "#6B7180"
  border: "rgba(255, 255, 255, 0.20)"
  border-blue: "rgba(73, 140, 255, 0.55)"
  card-bg: "rgba(255, 255, 255, 0.09)"
  card-bg-blue: "rgba(23, 95, 255, 0.16)"
  gradient: "linear-gradient(135deg, #49BCFF 0%, #175FFF 30%, #7F47FF 65%, #C84CFF 100%)"
  gradient-hero: "linear-gradient(135deg, #80F0E0 0%, #49BCFF 20%, #175FFF 45%, #7F47FF 75%, #C84CFF 100%)"

typography:
  h1:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 700
    fontSize: "clamp(44.8px, 5vw, 67.2px)"
    lineHeight: 1.05
    letterSpacing: -0.03em
    color: "{colors.text}"
  h2:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 700
    fontSize: "clamp(28.8px, 3vw, 41.6px)"
    lineHeight: 1.1
    letterSpacing: -0.02em
    color: "{colors.text}"
  h3:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(17.6px, 1.8vw, 24px)"
    lineHeight: 1.3
    letterSpacing: -0.01em
    color: "{colors.text}"
  h4-eyebrow:
    fontFamily: "'IBM Plex Mono', monospace"
    fontWeight: 500
    fontSize: "clamp(12.8px, 1.1vw, 15.2px)"
    lineHeight: 1.1
    letterSpacing: 0.12em
    textTransform: uppercase
    color: "{colors.sky}"
  body:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 400
    fontSize: "clamp(13.6px, 1.1vw, 16.8px)"
    lineHeight: 1.6
    color: "{colors.text-muted}"
  metric-value:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 700
    fontSize: "clamp(35.2px, 3.6vw, 52px)"
    lineHeight: 1
    letterSpacing: -0.02em
    color: "{colors.text}"
  metric-label:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(15.2px, 1.3vw, 17.6px)"
    lineHeight: 1.3
    color: "{colors.text}"
  metric-desc:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 400
    fontSize: "clamp(12.5px, 0.95vw, 14.4px)"
    lineHeight: 1.5
    color: "{colors.text-muted}"
  mono-label:
    fontFamily: "'IBM Plex Mono', monospace"
    fontWeight: 400
    fontSize: "clamp(11.2px, 0.95vw, 13.6px)"
    lineHeight: 1.4
    letterSpacing: 0.06em
    color: "{colors.text-light}"
  code:
    fontFamily: "'IBM Plex Mono', monospace"
    fontWeight: 400
    fontSize: "clamp(12.8px, 1.05vw, 15.2px)"
    lineHeight: 1.7
    color: "{colors.sky}"
  blockquote:
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: "clamp(25.6px, 2.8vw, 38.4px)"
    lineHeight: 1.3
    letterSpacing: -0.02em
    color: "{colors.text}"
  tag:
    fontFamily: "'IBM Plex Mono', monospace"
    fontWeight: 500
    fontSize: 12px
    lineHeight: 1
    letterSpacing: 0.08em
    textTransform: uppercase
    color: "{colors.sky}"
  counter:
    fontFamily: "'IBM Plex Mono', monospace"
    fontWeight: 400
    fontSize: 12.8px
    lineHeight: 1
    letterSpacing: 0.08em
    color: "{colors.text-muted}"
  meta:
    fontFamily: "'IBM Plex Mono', monospace"
    fontWeight: 400
    fontSize: 12.8px
    lineHeight: 1.4
    letterSpacing: 0.06em
    color: "{colors.text-light}"

spacing:
  pad-slide-x: "4vw"
  pad-slide-y-top: "3.5vw"
  pad-slide-y-bottom: "8.5vh"
  pad-card-lg: "1.6rem 1.7rem"
  pad-card-md: "1.4rem 1.5rem"
  pad-card-sm: "1rem 1.2rem"
  gap-grid-lg: "3.5rem"
  gap-grid-md: "2rem 3rem"
  gap-grid-sm: "1.5rem"
  gap-cards: "1.2rem"
  header-margin: "2.5vh"
  accent-line-width: "60px"
  accent-line-height: "4px"

canvas:
  width: 100vw
  height: 100vh
  background: "{colors.bg}"

radii:
  pill: "100px"
  card-lg: "16px"
  card-md: "12px"
  card-sm: "10px"
  bar: "6px"
  circle: "50%"

components:
  card:
    background: "{colors.card-bg}"
    border: "1px solid {colors.border}"
    borderRadius: 16px
    padding: "1.6rem 1.7rem"
    description: "Primary content card. A clearly-lifted translucent white surface (9% white) with a 20% white hairline border and 16px radius on the black canvas. No drop shadow — elevation reads from the translucent fill + hairline."
  card-blue:
    background: "{colors.card-bg-blue}"
    border: "1px solid {colors.border-blue}"
    borderRadius: 16px
    padding: "1.6rem 1.7rem"
    description: "Accent variant of the content card, tinted Zilliz Blue at 16% with a 55% blue border. Used to single out a focal card (a headline metric, a primary feature)."
  gradient-cta:
    background: "{colors.gradient}"
    color: "#FFFFFF"
    padding: "0.9rem 2.2rem"
    borderRadius: 100px
    fontFamily: "'Inter', sans-serif"
    fontWeight: 600
    fontSize: 15.2px
    description: "Primary CTA: a full-gradient pill in the Zilliz brand gradient with white text and 100px radius. Hover lifts -2px with a soft blue glow (0 8px 28px rgba(23,95,255,0.35)). The deck's single solid-gradient interactive element."
  tag-pill:
    background: "{colors.card-bg-blue}"
    color: "{colors.sky}"
    border: "1px solid {colors.border-blue}"
    padding: "0.35rem 0.9rem"
    borderRadius: 100px
    fontFamily: "'IBM Plex Mono', monospace"
    fontWeight: 500
    fontSize: 12px
    textTransform: uppercase
    description: "Mono tag pill in the top-right of the slide-header. Blue-tinted fill, blue border, sky-blue mono text, fully rounded."
  accent-line:
    width: 60px
    height: 4px
    background: "{colors.gradient}"
    borderRadius: 2px
    description: "Short 60×4 horizontal rule painted with the brand gradient. Sits above cover titles and as an eyebrow separator. The compact signature of the system."
  gradient-text:
    background: "{colors.gradient}"
    description: "Gradient-clipped text (background-clip: text; color: transparent). Reserved for one hero phrase per cover/section and for large metric values. Never apply to body or to a whole headline — only the emphasis word(s)."
  bar-track:
    height: 28px
    background: "{colors.card-bg}"
    border: "1px solid {colors.border}"
    borderRadius: 6px
    description: "Horizontal bar chart track: translucent white fill with a hairline border, 6px radius."
  bar-fill:
    height: "100%"
    background: "{colors.gradient}"
    borderRadius: 6px
    description: "Gradient fill inside bar-track. Width carries the data value; animates from 0 on slide entry."
  vector-lines:
    description: "Abstract decoration: a loose fan of thin (1–1.5px) diagonal line segments of varying length in sky/blue/purple/berry, evoking vector coordinates. Atmospheric only, on cover/section/closing surfaces. This is NOT the Zilliz logomark and must never be arranged to resemble the twinkling-star symbol."
  gradient-arc:
    description: "A single thin curved arc stroke painted with the brand gradient, sweeping through open space on cover/closing surfaces. Decorative atmosphere, low opacity."
  glow-orb:
    description: "A large, heavily-blurred radial gradient orb (blue→purple) bled off a corner at low opacity to give the black canvas luminous depth. Atmospheric only; never behind body text at an opacity that hurts contrast."
  progress-bar:
    position: "fixed bottom 0 left 0"
    height: 3px
    background: "{colors.gradient}"
    description: "Thin gradient progress strip at the bottom edge, width grows with slide index."
  nav-btn:
    width: 44px
    height: 44px
    borderRadius: 50%
    border: "1px solid {colors.border-blue}"
    background: "{colors.card-bg-blue}"
    color: "{colors.sky}"
    description: "Circular 44px nav-arrow button. Hover fills with the gradient and turns the icon white. Disabled at 30% opacity on first/last slide."
---

## Frontend Slides Fixed-Stage Policy

When this design system is used by the `frontend-slides` skill, generate the final deck as a **fixed 1920×1080 stage** that scales uniformly to the browser viewport. The deck preserves a 16:9 canvas on every screen, including phones; it may letterbox or pillarbox, but it must not reflow slide content for mobile.

This policy has higher priority than any source-template responsive behavior described later in this file. Treat viewport-fluid values (`100vw`, `100vh`, `vw`, `vh`, `clamp()`) as design proportions to translate into 1920×1080 stage coordinates, not as live responsive rules in the generated deck. Use `deck-stage.js` or an equivalent inline stage scaler, and verify rendered screenshots for both text overflow and panel overlap.

## Overview

Zilliz Brand is the **official Zilliz design system** for decks that must read as on-brand: product launches, technical keynotes, investor and developer-facing presentations, and internal Zilliz communications. Its foundational premise is **one dark luminous ground + one expressive gradient**: a near-black canvas (`{colors.bg}` — `#000000`) lit by the signature Zilliz brand gradient that flows sky blue → blue → purple → berry. Solid **Zilliz Blue** (`{colors.primary}` — `#175FFF`) carries non-gradient accents (CTAs in solid contexts, borders, links, chart highlights); the gradient carries the hero moments (one hero phrase, key metric values, the accent line, bar fills, the progress bar).

The type system uses two open Google fonts in fixed roles. **Inter** (weights 300–700) is the display + body face — every headline, every paragraph, every metric numeral. **IBM Plex Mono** (weight 400–600) is the technical chrome face — eyebrows, tag pills, slide counters, mono labels, code, and any "vector database / engineering" register cue. The Inter / IBM Plex Mono pairing is the system's typographic signature: humanist-sans headlines over precise-mono labels reads as modern, technical, and trustworthy.

Depth is **luminous, not shadowed**. Cards are translucent white (`{colors.card-bg}` — white at 9%) with hairline borders (`{colors.border}` — white at 20%); the focal card uses a blue tint (`{colors.card-bg-blue}`). The black canvas gains depth from heavily-blurred gradient **glow orbs** bled off the edges, never from drop shadows on content. The only glow is the soft blue lift on the CTA hover.

**Key Characteristics:**
- Near-black ground (`{colors.bg}`) on every surface — luminous, never flat gray.
- The Zilliz brand gradient (`{colors.gradient}`) as the single expressive device — used for one hero phrase, metric values, the accent line, bar fills, and the progress bar.
- Solid Zilliz Blue (`{colors.primary}`) for non-gradient accents: links, borders, focal-card tint, solid chart marks.
- Inter (display + body) + IBM Plex Mono (eyebrows, labels, code, chrome) — never substitute either.
- Cards are translucent white at 9% with 20% white hairline borders and 16px radius. No drop shadows.
- Gradient-clipped hero text — applied only to the emphasis word(s), never a whole headline or body.
- Atmospheric decoration from abstract "vector coordinate" diagonal lines, thin gradient arcs, and blurred glow orbs.
- Persistent chrome: gradient progress bar at the bottom edge, mono slide-counter bottom-left, circular nav-arrows bottom-right.

## Logo Usage (NON-NEGOTIABLE)

The Zilliz logo and logomark are **off-limits to generation**. Do **not** draw, redraw, hand-code (SVG/CSS), AI-generate, approximate, or otherwise invent the Zilliz wordmark or the twinkling-star symbol. The symbol is a precise geometric construction (12 vector-coordinate lines at key angles 20°/30°/40°); recreating it is prohibited.

- **Only** use official logo files from `https://zilliz.com/brand-assets`. If the user supplies an official logo asset, embed it (e.g., base64) on the cover/closing slide.
- If no official asset is available, use the wordmark "Zilliz" set in Inter, or omit the logo entirely — **never** fabricate a mark.
- Approved color variants (from official packages only): **Gradient** (preferred for digital), **Black** (`#000000`), **White** (`#FFFFFF`).
- Never fade, recolor, stretch, rotate, drop-shadow, or place the logo over busy imagery.
- Clear space: 0.5X on the sides, 1X top/bottom (X = half the symbol height). Minimum height 24px; recommended 120 / 72 / 48px.
- The `vector-lines` decoration evokes vector coordinates but **must not** be arranged to resemble the star logomark.

## Card Contrast Floor (NON-NEGOTIABLE)

The near-black canvas makes low-alpha surfaces disappear on projectors, compressed screen-shares (Zoom/Meet/Teams), dimmed laptop panels, and most non-OLED external displays. Values that look elegant on a calibrated OLED render as "text floating on black" everywhere else. Hard floors when generating on `{colors.bg}`:

- **Card fills: never below 8% white** (`rgba(255,255,255,0.08)`). Default is `{colors.card-bg}` at 9%.
- **Hairline borders: never below 18% white** (`rgba(255,255,255,0.18)`). Default is `{colors.border}` at 20%.
- **Blue focal fills: never below 14% blue**; blue borders never below 45%. Defaults are 16% / 55%.
- **Ghost/decorative numerals and watermarks: never below 8% white** — below that they simply don't exist off-OLED.
- Hover states must land **at least 10 alpha points above** the resting border so the lift is perceptible.

**Verification step (required):** after generating, screenshot the rendered deck and confirm every card edge is visibly separable from the canvas at a glance — then mentally subtract one brightness notch (projector test). If a card reads only by its text, raise the fill/border until the surface itself reads. Do not ship a slide whose panels are distinguishable from the background only on the machine that generated them.

## Colors

### Palette

- **Bg** (`{colors.bg}` — `#000000`): The near-black canvas. Every surface rests on it. Brand-approved dark ground.
- **Navy** (`{colors.navy}` — `#061982`): Deep brand blue. Used for the darkest gradient stops, deep contrast panels, and glow-orb cores.
- **Primary / Zilliz Blue** (`{colors.primary}` — `#175FFF`): The signature solid accent. Links, solid CTAs, focal-card tint and border, solid chart marks, key inline emphasis.
- **Sky Blue** (`{colors.sky}` — `#49BCFF`): Highlight + secondary accent. Eyebrows, mono labels in accent state, code, the lightest gradient stop.
- **Purple** (`{colors.purple}` — `#7F47FF`): Gradient mid-stop and secondary accent.
- **Berry** (`{colors.berry}` — `#C84CFF`): Gradient end-stop and warm accent.
- **Green** (`{colors.green}` — `#00DCC6`): Success / positive accent only — confirmations, positive deltas. Not a general decorative color.
- **Text** (`{colors.text}` — `#FFFFFF`): Primary text on the dark ground — headlines, primary content, metric labels.
- **Text-muted** (`{colors.text-muted}` — `#A9B0C0`): Body paragraphs, descriptions — a cool gray that reads softer than white without disappearing.
- **Text-light** (`{colors.text-light}` — `#6B7180`): Tertiary metadata, mono captions, counters.
- **Border** (`{colors.border}` — white at 20%): Universal hairline border on translucent cards and chrome.
- **Border-blue** (`{colors.border-blue}` — blue at 55%): Accent border on focal cards, tag pills, nav-buttons.
- **Card-bg** (`{colors.card-bg}` — white at 9%): Universal translucent card fill.
- **Card-bg-blue** (`{colors.card-bg-blue}` — blue at 16%): Focal-card and pill fill.
- **Gradient** (`{colors.gradient}`): The brand gradient, `135deg`, sky → blue → purple → berry. The single expressive device.
- **Gradient-hero** (`{colors.gradient-hero}`): The luminous hero variant adding a teal lead-in (`#80F0E0`). Reserved for large hero/cover gradient fields and glow orbs.

### Defaults

- **Default surface background**: `{colors.bg}` — every surface starts on near-black.
- **Default headline color**: `{colors.text}` (`#FFFFFF`). The gradient is for emphasis word(s) only, not whole headlines.
- **Default body text color**: `{colors.text-muted}` (`#A9B0C0`).
- **Default eyebrow color**: `{colors.sky}` (`#49BCFF`), IBM Plex Mono, uppercase, 0.12em tracking.
- **Default card fill / border**: `{colors.card-bg}` + 1px `{colors.border}`. Focal cards use `{colors.card-bg-blue}` + `{colors.border-blue}`.
- **Default expressive accent (hero phrase, metric value, accent line, bar fill, progress bar)**: `{colors.gradient}`.
- **Default solid accent (links, solid CTA, focal tint, chart marks)**: `{colors.primary}`.
- **Default positive indicator**: `{colors.green}`.

Use the gradient **sparingly and deliberately** — one hero phrase per cover/section, metric values, the accent line, bar fills, progress bar. Over-applying the gradient (to body text, multiple headlines, every card) collapses its impact. Restraint is what makes it read as premium brand, not decoration.

## Typography

### Font Family Stack

**Inter** (Google Fonts, weights 300–700) is the display + body face: every h1–h3, every paragraph and list body, every metric numeral and label. Headlines run weight 700 with negative tracking (-0.02 to -0.03em); body runs weight 400 at line-height 1.6 in the muted cool gray.

**IBM Plex Mono** (Google Fonts, weights 400–600) is the technical chrome face: h4 eyebrows (uppercase, 0.12em tracking, sky blue), tag pills, slide counters, mono labels, code blocks, and any "engineering register" cue. The mono face is the system's recognizable technical signature — it's what makes a Zilliz deck read as a vector-database product rather than a generic SaaS pitch.

The roles are non-overlapping: Inter handles headlines and prose; IBM Plex Mono handles labels, chrome, and code. Don't cross the boundary — mono body reads as a terminal dump; Inter eyebrows lose the technical signal.

### Loading

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=IBM+Plex+Mono:wght@400;500;600;700&display=swap" rel="stylesheet">
```

### Typography Scale

| Token | Size (clamp / px) | Family | Weight | Use |
|---|---|---|---|---|
| `{typography.h1}` | 44.8–67.2px | Inter | 700 | Cover or closing title |
| `{typography.h2}` | 28.8–41.6px | Inter | 700 | Primary section headline per slide |
| `{typography.h3}` | 17.6–24px | Inter | 600 | Region / agenda-item title |
| `{typography.h4-eyebrow}` | 12.8–15.2px | IBM Plex Mono | 500 | Uppercase eyebrow in the slide-header (sky blue, 0.12em) |
| `{typography.body}` | 13.6–16.8px | Inter | 400 | Standard body paragraph |
| `{typography.metric-value}` | 35.2–52px | Inter | 700 | Large metric numeral (often gradient-clipped) |
| `{typography.metric-label}` | 15.2–17.6px | Inter | 600 | Metric label line |
| `{typography.metric-desc}` | 12.5–14.4px | Inter | 400 | Metric supporting description |
| `{typography.mono-label}` | 11.2–13.6px | IBM Plex Mono | 400 | Technical caption / coordinate label |
| `{typography.code}` | 12.8–15.2px | IBM Plex Mono | 400 | Code snippet / technical data (sky blue) |
| `{typography.blockquote}` | 25.6–38.4px | Inter | 600 | Quote-class headline body |
| `{typography.tag}` | 12px | IBM Plex Mono | 500 | Tag pill text in slide-header |
| `{typography.counter}` | 12.8px | IBM Plex Mono | 400 | Persistent slide counter |
| `{typography.meta}` | 12.8px | IBM Plex Mono | 400 | Cover meta line (date / confidential marker) |

### Signature Treatments

These are **non-optional whenever the corresponding element type is used**:

- **Every h4 eyebrow is IBM Plex Mono weight 500 in `{colors.sky}`, uppercase, 0.12em tracking.** The mono eyebrow is the system's most recognizable small chrome.
- **Every headline (h1–h3) is Inter weight 600–700 in `{colors.text}` white with negative tracking.** White headlines, not gradient — the gradient is reserved for the emphasis word(s) within a hero line.
- **Gradient-clipped text is applied only to one hero phrase per cover/section and to large metric values.** Never the whole headline, never body, never multiple phrases on one slide.
- **Every body paragraph is Inter weight 400 in `{colors.text-muted}` with line-height 1.6.** Body in pure white reads as too harsh on black; body in text-light reads as too faint.
- **Every CTA is the `{components.gradient-cta}` pattern: full-gradient pill, white text, 100px radius.** No other CTA shape exists.
- **Every slide-header places the mono eyebrow on the left and a tag pill on the right.** This is the structural rhythm of every content slide.
- **Code and technical data are IBM Plex Mono in `{colors.sky}` or white on a translucent card.** Never set code in Inter.

### Typography Principles

The voice contrast is **white Inter headlines ↔ sky-blue mono eyebrows + labels ↔ cool-gray Inter body ↔ gradient-clipped hero word**. Italic and underline are not used; emphasis comes from weight, the white→sky/gradient color shift, and uppercase+tracking on mono labels. Numerical content is Inter (not mono) so big metrics read as confident display figures; small technical/coordinate labels are mono.

## Layout

### Canvas System
The system targets `100vw × 100vh` per slide. Slides are absolutely positioned and animated in via opacity + translateX (40px → 0px) on 500ms ease. Only the `.active` slide is `opacity: 1`; the previous slide gets `.prev` and translates -40px out.

Default slide padding is asymmetric: `3.5vw` left/top/right; `8.5vh` bottom, reserving room for the fixed slide-counter (left) and nav-controls (right) at `bottom: 2.5vh`.

### Padding and Gap Scale

| Token | Value | Use |
|---|---|---|
| `{spacing.pad-slide-x}` | 4vw | Slide horizontal padding |
| `{spacing.pad-slide-y-top}` | 3.5vw | Slide top padding |
| `{spacing.pad-slide-y-bottom}` | 8.5vh | Slide bottom padding (clears nav chrome) |
| `{spacing.pad-card-lg}` | 1.6rem 1.7rem | Large card internal padding |
| `{spacing.pad-card-md}` | 1.4rem 1.5rem | Medium card internal padding |
| `{spacing.pad-card-sm}` | 1rem 1.2rem | Small card internal padding |
| `{spacing.gap-grid-lg}` | 3.5rem | Gap between split columns |
| `{spacing.gap-grid-md}` | 2rem 3rem | Gap in two-column grids (row × col) |
| `{spacing.gap-grid-sm}` | 1.5rem | Gap in 3-column metric grids |
| `{spacing.gap-cards}` | 1.2rem | Gap between dashboard cells |
| `{spacing.header-margin}` | 2.5vh | Margin below the slide-header |

### Persistent Chrome
Three elements appear on every slide:
- **Slide counter** bottom-left — IBM Plex Mono 12.8px in text-muted, fixed at `bottom: 2.5vh; left: 3vw`.
- **Nav controls** bottom-right — two circular 44px `{components.nav-btn}` with blue hairline borders, fixed at `bottom: 2.5vh; right: 3vw`. Disabled at 30% opacity on first/last slide.
- **Progress bar** bottom edge — 3px gradient strip with width = `(currentSlide + 1) / total * 100%`.

### Slide-Header Structure
Every content slide carries a `.slide-header` band: a mono eyebrow on the left, a tag pill on the right. Below sits the section h2, then the content region (grid, list, chart, code, or split). Cover, quote, and closing slides skip the header in favor of centered content.

### Content Grids
Repeated grid patterns carry content density: 2×3 agenda grid, 3-column metric row, 3-column stat grid, split-body (1.05fr / 1fr), step/timeline row, 2-column detail grid. Grid choice follows content volume, not a fixed layout vocabulary.

## Depth and Elevation

### Translucent Cards (Primary Depth Mechanism)
Cards use `background: {colors.card-bg}` (white at 9%) + `border: 1px solid {colors.border}` (white at 20%) + 16px radius. They lift off the black ground without any offset. The focal card swaps to `{colors.card-bg-blue}` + `{colors.border-blue}` to pull one element forward.

### Glow Orbs, Not Shadows
There are no `box-shadow` declarations on content. Depth on the black canvas comes from large, heavily-blurred radial gradient **glow orbs** (blue→purple, `{colors.gradient-hero}` cores) bled off the edges at low opacity. The only shadow in the system is the soft blue glow on CTA hover: `0 8px 28px rgba(23, 95, 255, 0.35)`.

### Gradient as Structural Accent
The brand gradient does the structural-accent work that a colored rule or shadow would do elsewhere: the 60×4 accent line, bar fills, the progress bar, and the one gradient-clipped hero phrase all anchor the eye. Used sparingly, the gradient is the system's depth and focus device.

## Shapes and Treatment

### Border Radius
- **`{radii.pill}` = 100px** — `{components.gradient-cta}`, `{components.tag-pill}`, pill chrome.
- **`{radii.card-lg}` = 16px** — content cards.
- **`{radii.card-md}` = 12px** — compact cards, code blocks.
- **`{radii.card-sm}` = 10px** — mini cells.
- **`{radii.bar}` = 6px** — bar tracks/fills.
- **`{radii.circle}` = 50%** — nav buttons, dots, decorative circles.

No square (0px) corners anywhere except the progress bar.

### Border Weights
- **1px `{colors.border}`** (white 20%) — universal hairline on cards, code blocks, mini cells.
- **1px `{colors.border-blue}`** (blue 55%) — focal cards, tag pills, nav-buttons.
- Borders are **never opaque** — translucency is what gives the dark system its luminous, lifted quality.

### Decorative Element Types

**Translucent card** (`{components.card}`) — white-at-9% fill, white-at-20% hairline, 16px radius. The primary content card.

**Tag pill** (`{components.tag-pill}`) — blue-tinted mono pill in the slide-header top-right.

**Eyebrow** (`{typography.h4-eyebrow}`) — uppercase sky-blue mono label, 0.12em tracking, top-left of the slide-header.

**Gradient CTA** (`{components.gradient-cta}`) — full-gradient pill with white text. The system's one solid-gradient interactive element.

**Accent line** (`{components.accent-line}`) — a 60×4 gradient rule above cover titles and as an eyebrow separator.

**Gradient-clipped text** (`{components.gradient-text}`) — one hero phrase or a metric value painted with the brand gradient via `background-clip: text`.

**Bar track + fill** (`{components.bar-track}` + `{components.bar-fill}`) — translucent track with a gradient fill whose width carries data; 6px radius.

**Vector lines** (`{components.vector-lines}`) — abstract diagonal coordinate-line decoration in sky/blue/purple/berry. Atmospheric only; never the logomark.

**Gradient arc** (`{components.gradient-arc}`) — a thin gradient-stroked curve through open space on cover/closing surfaces.

**Glow orb** (`{components.glow-orb}`) — a large blurred radial gradient bled off a corner for luminous depth.

## Do's and Don'ts

### Do

- Apply `{colors.bg}` (`#000000`) as the universal canvas. Every surface starts on near-black.
- Use the brand gradient (`{colors.gradient}`) as the single expressive device — one hero phrase, metric values, accent line, bar fills, progress bar.
- Use solid Zilliz Blue (`{colors.primary}`) for non-gradient accents: links, solid CTAs in tight spots, focal-card tint, solid chart marks.
- Set headlines in `{colors.text}` white with negative tracking; gradient-clip only the emphasis word(s).
- Set every eyebrow in IBM Plex Mono, uppercase, 0.12em tracking, sky blue. The mono eyebrow is the universal section opener.
- Use `{components.card}` (white-at-9% + white-at-20% hairline + 16px radius) as the universal content card; promote one focal card with the blue variant.
- Set body in Inter weight 400 in `{colors.text-muted}` with line-height 1.6.
- Set code and technical data in IBM Plex Mono in sky blue or white on a translucent card.
- Use `{colors.green}` only for genuine positive/success indicators.
- Give the black canvas luminous depth with blurred glow orbs and abstract vector-line decoration.

### Don't

- Don't recreate, hand-code, or AI-generate the Zilliz logo or star logomark in any form. Use official assets only, or omit.
- Don't over-apply the gradient — not on body, not on multiple headlines, not on every card. One expressive hero moment per surface.
- Don't gradient-clip an entire headline; only the emphasis word(s).
- Don't use drop shadows on cards or content. Depth is translucency + glow orbs, never offset shadows.
- Don't use opaque borders. Borders are translucent white-at-10% or blue-at-35%.
- Don't substitute fonts. Inter + IBM Plex Mono is the pairing; Roboto, Open Sans, or Arial collapse the identity.
- Don't set body or headlines in mono, and don't set code or labels in Inter — the face roles are fixed.
- Don't switch the canvas to white or gray per slide; the constant near-black ground is the system's identity.
- Don't arrange the vector-line decoration to resemble the star logomark.
- Don't use green/purple/berry as general decorative fills outside the gradient and their defined accent roles.

## Responsive Behavior

Zilliz Brand is a **1920×1080 presentation system** (effective 100vw × 100vh). Type uses `clamp()`; spacing uses `vw / vh / rem`. A single `@media (max-height: 700px)` block tightens slide padding and card padding on dense slides. Slides advance via `ArrowRight` / `Space` / `PageDown`, reverse via `ArrowLeft` / `PageUp`, with `Home`/`End` jumps and a 50px horizontal touch-swipe threshold. Transitions are 500ms ease (opacity fade + 40px translateX). The progress bar animates to the current slide percentage over 400ms.

### Interactive States
- Nav-buttons fill with the gradient on hover (icon turns white).
- Cards lift subtly on hover via a 1px brighter border (white 20% → 32%), no shadow.
- CTA lifts -2px on hover with the soft blue glow (`0 8px 28px rgba(23,95,255,0.35)`).
- Bar fills animate from 0 to value over 0.8s on slide entry.

## CJK & International Content

For Chinese (or other CJK) content, swap the Latin stack for a CJK pairing loaded via CDN and apply universal CJK adjustments.

### Recommended Chinese Pairing

| Role | Latin (default) | Chinese counterpart |
|---|---|---|
| Headlines / body / metrics | Inter | 思源黑体 Noto Sans SC 400–700 |
| Eyebrows / labels / code / chrome | IBM Plex Mono | 思源黑体 Noto Sans SC 500 (no transform) or keep IBM Plex Mono for Latin/digits in code |

### Loading

```html
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@400;500;600;700&family=IBM+Plex+Mono:wght@400;500;600&display=swap" rel="stylesheet">
```

### Universal CJK Adjustments
- **Line-height**: increase ~15–25% (body 1.75–1.85, display 1.2–1.3). CJK glyphs crowd vertically.
- **Letter-spacing**: set to 0 on every CJK run. The −0.02/−0.03em headline tracking overlaps CJK strokes; the +0.12em eyebrow tracking reads gappy on square glyphs.
- **Text transform**: don't apply `uppercase` to Chinese — CJK has no case. Remove it on the eyebrow and tag tokens for CJK runs.
- **Punctuation**: use full-width Chinese punctuation （，。：；！？「」（））.
- **Space between CJK and Latin (盘古之白)**: insert an ASCII space between Chinese characters and adjacent Latin/digits — write `Zilliz Cloud 向量数据库`, `每秒 10000 QPS`.
- **Keep numerals and code Latin**: metric figures and code stay Latin digits / IBM Plex Mono by convention; the gradient-clip on metric values still applies.

### Aesthetic Notes
The identity — near-black ground, one brand gradient, mono labels, luminous depth — transfers cleanly to CJK. The mono eyebrow loses its uppercase+tracking signal in 思源黑体; compensate by always pairing the eyebrow with the gradient `{components.accent-line}` so the gradient rule carries chrome recognition. Keep the eyebrow in sky blue.

## Iteration Guide

1. Any new slide starts on `{colors.bg}` near-black. The constant ground is the identity.
2. Any new content slide carries a slide-header: mono eyebrow (sky blue, uppercase, 0.12em) left + tag pill right.
3. Any new headline is Inter weight 600–700 in white with negative tracking; gradient-clip only the emphasis word.
4. Any new card uses `{components.card}` (white-at-9% + white-at-20% hairline + 16px). Promote one focal card with the blue variant.
5. Any new metric value is Inter weight 700, gradient-clipped, with an Inter label and muted-gray description.
6. Any new accent line, bar fill, or progress indicator uses the brand gradient.
7. Any new CTA uses `{components.gradient-cta}` — full-gradient pill, white text, 100px radius.
8. Any new code/technical block is IBM Plex Mono in sky blue/white on a translucent card.
9. Any new decoration is abstract vector lines, a gradient arc, or a glow orb — never the logomark.
10. If a surface feels sparse, add a glow orb or vector-line decoration and real content — don't over-apply the gradient to fill space.

## Known Gaps

- **Inter and IBM Plex Mono load from Google Fonts** via preconnect + `<link>`. In environments where Google Fonts fail, the system collapses to `sans-serif` / `monospace` and loses character.
- **The logo cannot be generated.** Without an official brand-asset file, the cover/closing uses the "Zilliz" wordmark in Inter or omits the mark entirely. This is intentional brand protection, not a limitation to work around.
- **The gradient is contrast-sensitive on text.** Gradient-clipped text over the berry/purple end can dip in contrast against black at small sizes; reserve gradient-clip for large hero/metric type, keep small text white/sky.
- **Low-alpha surfaces vanish off-OLED.** Earlier versions of this system used 4% card fills and 10% borders; on projectors and compressed screen-shares those are indistinguishable from the black canvas. The tokens now sit at 9%/20% — treat those as floors, not suggestions (see "Card Contrast Floor").
- **Glow orbs can wash out body contrast** if placed behind paragraphs at high opacity; keep them off content regions or at low opacity.
- **The single-gradient discipline limits categorical color encoding.** Multi-series charts should distinguish via solid blue/sky/purple/berry/green marks (their defined roles) rather than inventing new hues.
