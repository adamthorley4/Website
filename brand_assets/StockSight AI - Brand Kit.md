# StockSight AI — Brand Kit

> A self-contained brand reference for use with designers, developers, agencies, or any external tool or platform. Everything needed to implement the StockSight AI brand consistently.

---

## Identity

| | |
|---|---|
| **Company name** | StockSight AI |
| **Primary tagline** | See the signal before the move. |
| **Product tagline** | Understand what's moving markets — instantly. |
| **Category** | Real-time market intelligence · Fintech · AI |
| **One-line description** | StockSight AI detects market-moving signals in real time and explains their potential impact before the broader market fully reacts. |

---

## Colours

### Core Palette

| Role | Hex | Notes |
|------|-----|-------|
| Primary green | `#00D68F` | Emerald. CTAs, bullish signals, positive trends, gradient start |
| Primary blue | `#2979FF` | Electric blue. Links, secondary CTAs, informational, gradient end |
| Background | `#0D0D1A` | Deep navy. All primary surfaces |
| Surface | `#13131F` | Elevated cards, panels, modals |
| Border | `#1E1E30` | Dividers, outlines, card edges |
| Text primary | `#FFFFFF` | Headlines, high-emphasis copy |
| Text secondary | `#A0A0B8` | Supporting copy, labels, metadata |
| Text disabled | `#5A5A72` | Disabled states, placeholders |

### Gradient

`#00D68F` → `#2979FF` — applied left-to-right or top-left to bottom-right.
Used on: logo, hero sections, primary CTAs, signal glows, key graphic accents.

### Semantic Colours

| Signal | Hex | Usage |
|--------|-----|-------|
| Bullish / Positive | `#00D68F` | Upward price moves, buy signals, positive delta |
| Bearish / Negative | `#FF4D6A` | Downward price moves, sell signals, negative delta |
| Warning | `#FFB547` | Moderate confidence, caution alerts |
| Info | `#2979FF` | Informational notices |
| Neutral | `#A0A0B8` | Unchanged, loading, indeterminate |

### Rules

- Dark-first. Every surface starts from `#0D0D1A`. No light or white backgrounds.
- The gradient is reserved for high-impact elements — do not use it decoratively.
- Body text should be `#FFFFFF` at 90–95% opacity (not pure white) to reduce eye strain on dark.

---

## Typography

### Fonts

| Role | Font | Weights | Source |
|------|------|---------|--------|
| Display / Hero titles | **Space Grotesk** | 600, 700 | [fonts.google.com/specimen/Space+Grotesk](https://fonts.google.com/specimen/Space+Grotesk) |
| Body / UI text | **Inter** | 400, 500, 600 | [fonts.google.com/specimen/Inter](https://fonts.google.com/specimen/Inter) |
| Data / Tickers / Prices | **IBM Plex Mono** | 400, 500 | [fonts.google.com/specimen/IBM+Plex+Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) |

All fonts are free and open-source (SIL Open Font Licence) via Google Fonts.

### CSS Import

```css
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@600;700&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap');
```

### CSS Variables

```css
:root {
  --font-display: 'Space Grotesk', -apple-system, BlinkMacSystemFont, sans-serif;
  --font-body:    'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
  --font-mono:    'IBM Plex Mono', 'Courier New', monospace;
}
```

### Type Scale

| Level | Font | Weight | Desktop size | Mobile size |
|-------|------|--------|-------------|-------------|
| Hero | Space Grotesk | 700 | 56–72px | 36–48px |
| H1 | Space Grotesk | 700 | 40px | 28px |
| H2 | Space Grotesk | 600 | 28px | 22px |
| H3 | Inter | 600 | 20px | 18px |
| H4 | Inter | 600 | 16px | 15px |
| Body large | Inter | 400 | 18px | 16px |
| Body | Inter | 400 | 15–16px | 14px |
| Body small | Inter | 400 | 13px | 12px |
| UI label | Inter | 500 | 12–13px | 12px |
| Ticker | IBM Plex Mono | 500 | 14–16px | 13px |
| Price / data | IBM Plex Mono | 400–500 | 13–16px | 12–14px |

### Typography Rules

- Space Grotesk for Hero, H1, H2 only. Inter from H3 downwards.
- Line height: 1.4–1.5× for body. 1.1–1.2× for display headings.
- Letter spacing: `−0.02em` for large display text. `0.01em` for labels.
- Accent colour on text: `#00D68F` for positive data highlights. `#2979FF` for links and interactive elements. Not for long-form body copy.

---

## Logo

### Files

| File | Format | Usage |
|------|--------|-------|
| `StockSight Logo.jpeg` | JPEG | Icon mark only — favicons, app icons, watermarks |
| `StockSight Logo with name.jpeg` | JPEG | Standard logo — headers, documents, presentations |
| `StockSight Logo with slogan.jpeg` | JPEG | Full brand mark — splash screens, marketing |

### Rules

- Do not recolour, stretch, or alter the logo.
- Minimum clear space: equal to the height of the "S" mark on all four sides.
- Preferred placement on dark backgrounds only (`#0D0D1A` or similar).
- Watermark usage: 60–70% opacity, bottom-right or bottom-left corner.

---

## Visual Style

- **Aesthetic:** Dark mode, premium fintech, futuristic — not aggressive or hype-driven.
- **Motifs:** Candlestick charts, upward trend lines, real-time data feeds, signal alerts, glowing neon-on-dark effects.
- **Mood:** Confident, intelligent, forward-moving.
- **Composition:** Clean negative space. Dark background dominant. Gradient accents as focal points.

---

## Voice & Tone

- **Intelligent, confident, minimal.** Short sentences. Active voice.
- **Audience:** Retail traders and investors who want to react faster and understand what is driving market moves.

### Use

- "See the signal before the move."
- "Understand what's moving markets — instantly."
- "React faster with real-time intelligence."
- "The cause, not just the outcome."

### Avoid

- Financial advice framing or profit guarantees
- Competitor comparisons
- Slang, hype, or urgency-baiting language
- Emojis in body copy

---

## Quick-Reference Card

```
Company:     StockSight AI
Tagline:     See the signal before the move.

Colours
  Green      #00D68F
  Blue       #2979FF
  Background #0D0D1A
  Surface    #13131F
  Bullish    #00D68F
  Bearish    #FF4D6A
  Text       #FFFFFF / #A0A0B8

Fonts
  Display    Space Grotesk  600, 700
  Body       Inter          400, 500, 600
  Data       IBM Plex Mono  400, 500
  (all via Google Fonts — free)

Style        Dark-first · Gradient green→blue · Premium fintech
```
