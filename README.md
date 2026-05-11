---
version: alpha
name: MPO Fantasy Football
description: >
  Visual identity system for MPO — a fantasy football franchise engineered
  beyond Earth. 70% elite sports franchise, 30% cosmic mystery.

colors:
  primary: "#7CFF3A"
  secondary: "#0F5A3C"
  neutral: "#FFFFFF"
  void: "#050A07"
  on-primary: "#050A07"
  on-secondary: "#7CFF3A"
  on-neutral: "#0F5A3C"

typography:
  h1:
    fontFamily: Rajdhani
    fontSize: 3rem
    fontWeight: 700
    letterSpacing: 0.02em
    lineHeight: 1.05
  h2:
    fontFamily: Rajdhani
    fontSize: 2rem
    fontWeight: 700
    letterSpacing: 0.02em
    lineHeight: 1.1
  h3:
    fontFamily: Rajdhani
    fontSize: 1.5rem
    fontWeight: 600
    letterSpacing: 0.01em
    lineHeight: 1.2
  body-md:
    fontFamily: Rajdhani
    fontSize: 1rem
    fontWeight: 500
    lineHeight: 1.5
  label-caps:
    fontFamily: Rajdhani
    fontSize: 0.75rem
    fontWeight: 600
    letterSpacing: 0.12em
    lineHeight: 1.4
  stat:
    fontFamily: Rajdhani
    fontSize: 2.5rem
    fontWeight: 700
    letterSpacing: 0.01em
    lineHeight: 1

rounded:
  none: 0px
  sm: 2px
  md: 4px
  lg: 8px

spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  2xl: 64px

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-caps}"
    rounded: "{rounded.sm}"
    padding: "12px 24px"
  button-primary-hover:
    backgroundColor: "#9FFF62"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.primary}"
    rounded: "{rounded.sm}"
    padding: "11px 23px"
  button-secondary-hover:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.primary}"
  badge:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.primary}"
    typography: "{typography.label-caps}"
    rounded: "{rounded.sm}"
    padding: "4px 10px"
  card:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  card-hover:
    backgroundColor: "#1A6B49"
    textColor: "{colors.neutral}"
  stat-block:
    backgroundColor: "{colors.void}"
    textColor: "{colors.primary}"
    typography: "{typography.stat}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  nav:
    backgroundColor: "{colors.void}"
    textColor: "{colors.neutral}"
    typography: "{typography.label-caps}"
  nav-active:
    textColor: "{colors.primary}"
  input:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.sm}"
    padding: "10px 16px"
  input-focus:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.neutral}"
---

## Overview

MPO is a premium fantasy football franchise built on the concept of
extraterrestrial dominance — the franchise an advanced civilization would
engineer to systematically dismantle human competition.

The identity balances **elite sports franchise energy** with **cosmic
intelligence**. Every surface should feel like it was produced by a
civilization operating several technological generations ahead of us: calm,
methodical, and impossibly precise. Never cartoonish. Never chaotic.

**Creative philosophy:** "A professional football organization designed by an
advanced extraterrestrial civilization."

The ratio is fixed:
- 70% elite sports franchise
- 30% cosmic mystery

Never reverse that ratio. The brand fails when the alien aesthetic overtakes
the athletic credibility.

**Brand personality axes:**
- Elite → feels like a championship franchise
- Futuristic → advanced beyond human technology
- Tactical → military precision and discipline
- Mysterious → hidden origins, cosmic intelligence
- Aggressive → dominant competitive identity
- Premium → high-end execution and restraint

---

## Colors

The palette contains exactly four colors. No additional hues are approved.
Color ratios are enforced: 60% void/deep green ground, 30% white type,
10% neon accent. Neon is a punch, not a wash.

- **Primary (#7CFF3A — Neon Pulse):** The signal. Used for highlights, key
  numbers, CTAs, logo marks, active states, and any element that must read
  as alive. Never use as a background at large scale — it will overwhelm the
  system. Neon earns its place by contrast, not coverage.

- **Secondary (#0F5A3C — Deep Field):** The ground. Primary uniform color,
  helmet shells, card backgrounds, deep environment fills. Conveys the
  alien-green darkness of a stadium at night. The brand lives here.

- **Neutral (#FFFFFF — Pure Signal):** Away kit and high-contrast contexts.
  Logo outlines, type on dark backgrounds. Provides the clean read on deep
  field. Do not tint; use at full white only.

- **Void (#050A07 — Deep Void):** Shadow, depth, studio backgrounds. Optional
  but preferred for maximum contrast behind neon. Slightly warmer than pure
  black, preserving a green undertone even in the darkest surfaces.

**Approved combinations:**

| Foreground | Background | Usage |
|---|---|---|
| Primary (neon) | Void | Max contrast, hero moments |
| Primary (neon) | Secondary (deep field) | Standard UI, cards |
| Neutral (white) | Secondary (deep field) | Body type on dark |
| Secondary (deep field) | Neutral (white) | Away / light mode |
| On-primary (void) | Primary (neon) | Button labels on neon fill |

---

## Typography

The single approved typeface is **Rajdhani**, designed by Indian Type
Foundry. It is wide, athletic, and geometric without decorative flourish —
it reads as engineered, not expressive.

**Weight system:**

| Weight | Token | Use |
|---|---|---|
| 500 Medium | `body-md` | Paragraphs, captions, labels |
| 600 SemiBold | `h3`, `label-caps` | Subheads, nav, button labels, table headers |
| 700 Bold | `h1`, `h2`, `stat` | Headlines, scoreboards, stat callouts only |

**Rules:**
- Always uppercase for headlines and label-caps contexts.
- Prefer wide spacing (`letter-spacing: 0.12em`) on caps labels.
- Never use decorative or display fonts as alternatives.
- Fallback stack: `'Rajdhani', 'Arial Narrow', sans-serif`.
- Import via: `https://fonts.google.com/specimen/Rajdhani`

---

## Layout

The grid is structured for dark environments. Layouts must breathe —
whitespace (void space) is part of the intimidation aesthetic.

**Principles:**
- Content never crowds the edge. Minimum horizontal margin is `spacing.xl`
  on desktop, `spacing.md` on mobile.
- Sections are separated with generous negative space, not dividers.
- Asymmetry is allowed and encouraged at the macro level (e.g., logo left,
  content right), but micro-elements (numbers, badges) must be optically
  centered.

**Grid reference:**
- Desktop: 12-column, 24px gutters, 40px outer margins
- Mobile: 4-column, 16px gutters, 16px outer margins
- Max content width: 1280px

**Spacing scale usage:**
- `xs (4px)`: Inline icon gaps, tight label spacing
- `sm (8px)`: Input internal spacing, badge padding
- `md (16px)`: Card internal sections
- `lg (24px)`: Card padding, section sub-groups
- `xl (40px)`: Section margins, hero padding
- `2xl (64px)`: Top-level section separation

---

## Elevation & Depth

MPO uses atmospheric depth, not traditional material elevation shadows.
The system operates in dark space — light comes from the content, not
from simulated environmental sources.

**Depth layers:**

| Layer | Treatment |
|---|---|
| Base | `void` background, no shadow |
| Card | Deep field surface, 1px `primary` border at 15% opacity |
| Active / focused | 1px `primary` border at 60% opacity, subtle outer glow: `0 0 12px rgba(124,255,58,0.25)` |
| Hero / modal | Backdrop blur + deep void overlay at 85% opacity |

**Glow discipline:** Neon glow effects are permitted only on the primary
logo, active interactive states, and intentional hero moments. Never apply
glow to body text, background fills, or decorative elements. One glowing
element per visual frame is the maximum.

---

## Shapes

The MPO visual language is built on precision geometry. Organic, rounded,
or playful shapes are not approved.

- **Border radius:** Near-zero preferred (`rounded.sm: 2px`, `rounded.md: 4px`).
  Cards and containers use `4px` maximum. Pill shapes are not approved.
- **Lines and dividers:** 1px, `primary` at reduced opacity, or omitted
  entirely in favor of spatial separation.
- **Iconography:** Geometric and minimal. The alien glyph language (center
  helmet stripe, pant stripe) is a canonical asset — never substitute or
  redesign individual characters. The glyph system follows a vertical flow
  and must never resemble Earth alphabets.
- **Logo clear space:** Minimum 1× cap-height on all sides of the primary
  mark. Do not crowd it.

**Secondary marks (fixed use cases, no substitution):**

| Mark | Token | Use |
|---|---|---|
| Primary alien head | `MPO-PRI-01` | Helmet side, pants, main logo |
| Flying saucer | `MPO-SEC-01` | Merchandise, social, motion |
| Zeta Reticuli star chart | `MPO-SEC-02` | Jersey upper back, shoulder patch |
| Movimientos wordmark | `MPO-SEC-03` | Limited apparel, Ritual of Ondulant campaign |

---

## Components

### Buttons

**Primary button** (`button-primary`): Neon Pulse fill, Deep Void text,
Rajdhani SemiBold label-caps, 2px radius. This is the single approved CTA
surface. Never use on a light background — it loses legibility against white.

**Secondary button** (`button-secondary`): Transparent fill, 1px Neon Pulse
border, Neon Pulse text. Used for secondary actions alongside a primary CTA.
Never use two primary buttons in the same view.

### Cards

Dark field surfaces with optional neon border accent. Padding follows
`spacing.lg`. Headers use `h3`, body uses `body-md` in neutral white.
Active or highlighted cards gain a 1px neon border at 60% opacity.

### Stat Blocks

Score, rank, and performance numbers use the `stat` typography token
(Rajdhani 700, 2.5rem) in Neon Pulse on Void. This is the only context where
neon is used at large scale — the numbers earn it by being data.

### Navigation

`label-caps` weight, spaced tracking, neutral white at rest, neon on active.
Background is always Deep Void. No underlines. Active state is color-only.

### Inputs

Deep Field background, neutral white text, 2px radius. Focus state gains
the standard neon border glow. Placeholder text at 50% neutral opacity.

---

## Do's and Don'ts

### ✅ Do

- Use Neon Pulse as a precision accent — numbers, logos, active states
- Keep backgrounds in the Deep Void / Deep Field range
- Apply uppercase tracking on all label and headline typography
- Use the alien glyph stripe exactly as specified — no character substitution
- Maintain the 70/30 sports-to-cosmic ratio in all layouts
- Apply atmospheric depth (glow, fog) sparingly and only on hero moments
- Place only one primary logo per surface; no duplicates

### ❌ Don't

- Use more than one glowing element per frame
- Apply neon as a background fill at large scale
- Round corners beyond `4px`
- Use any typeface other than Rajdhani
- Recolor the logo outside the approved palette
- Rotate or stretch the primary mark
- Add gradients to the primary alien head logo
- Use cartoon or playful visual references
- Crowd layouts — negative space is a feature, not wasted space
- Create new secondary marks without brand approval
- Mix inconsistent green tones — only `#7CFF3A`, `#0F5A3C`, and `#050A07`
- Apply random sci-fi effects (heavy glitch, excessive particles, chaotic motion)
