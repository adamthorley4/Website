# StockSight AI — Brand Style Guide

> This document defines the visual and typographic standards for StockSight AI. Follow these specifications consistently across all product, marketing, and content touchpoints.

---

## 1. Colours

### Core Palette

| Role | Name | Hex | Usage |
|------|------|-----|-------|
| Primary accent | Emerald green | `#00D68F` | CTAs, positive signals, upward trends, highlights |
| Secondary accent | Electric blue | `#2979FF` | Links, secondary CTAs, informational elements, hover states |
| Gradient | Green → Blue | `#00D68F` → `#2979FF` | Logo, hero elements, key graphic accents (left-to-right or top-left → bottom-right) |
| Background | Deep navy | `#0D0D1A` | Primary background across all surfaces |
| Surface | Elevated dark | `#13131F` | Cards, panels, modals — one step above background |
| Border | Subtle line | `#1E1E30` | Dividers, card borders, input outlines |
| Text primary | White | `#FFFFFF` | Headlines and high-emphasis body text |
| Text secondary | Muted white | `#A0A0B8` | Supporting copy, labels, metadata |
| Text disabled | Dim | `#5A5A72` | Disabled states, placeholder text |

### Semantic Colours

| Signal | Hex | Usage |
|--------|-----|-------|
| Bullish / Positive | `#00D68F` | Upward price movements, buy signals, positive delta |
| Bearish / Negative | `#FF4D6A` | Downward price movements, sell signals, negative delta |
| Neutral / Pending | `#A0A0B8` | Unchanged, loading, indeterminate states |
| Warning | `#FFB547` | Caution alerts, moderate-confidence signals |
| Info | `#2979FF` | Informational notices, secondary alerts |

### Colour Rules

- **Dark-first.** Every surface starts from `#0D0D1A`. Never use white or light backgrounds.
- The green-to-blue gradient is reserved for high-impact moments — logo, hero sections, primary CTAs, signal glows. Do not use it decoratively everywhere.
- Body text on dark backgrounds should use `#FFFFFF` at reduced opacity (≈ 90–95%) rather than pure white to reduce eye strain.
- Avoid placing `#00D68F` and `#2979FF` directly adjacent to each other outside of the gradient — it creates visual tension.

---

## 2. Typography

### Font Stack

| Role | Font | Weights | Source |
|------|------|---------|--------|
| Display / Hero titles | **Space Grotesk** | 600, 700 | [Google Fonts](https://fonts.google.com/specimen/Space+Grotesk) |
| Body / UI text | **Inter** | 400, 500, 600 | [Google Fonts](https://fonts.google.com/specimen/Inter) |
| Data / Tickers / Prices | **IBM Plex Mono** | 400, 500 | [Google Fonts](https://fonts.google.com/specimen/IBM+Plex+Mono) |

### Why These Fonts

**Space Grotesk** (display) has a slightly mechanical, engineered character — geometric but with subtle imperfections that give it personality. On a dark background with neon accents it reads as confident and technical without feeling clinical. Used widely across premium fintech and crypto products.

**Inter** (body/UI) is the de facto standard for professional trading interfaces. It was built specifically for screen rendering, has exceptional numeric clarity with tabular figures, and provides very high legibility at small sizes — essential for dense UI data.

**IBM Plex Mono** (data) is purpose-built for situations where character precision matters. It has tabular figures (all numbers are the same width, so prices align vertically), an unambiguous slashed zero, and clear l/1/I distinction — critical when displaying tickers, prices, and volumes.

### CSS Variables

```css
--font-display: 'Space Grotesk', -apple-system, BlinkMacSystemFont, sans-serif;
--font-body:    'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono:    'IBM Plex Mono', 'Courier New', monospace;
```

### Type Scale

| Level | Font | Weight | Size (desktop) | Size (mobile) | Usage |
|-------|------|--------|---------------|---------------|-------|
| Hero | Space Grotesk | 700 | 56–72px | 36–48px | Landing page headline, campaign title |
| H1 | Space Grotesk | 700 | 40px | 28px | Page titles |
| H2 | Space Grotesk | 600 | 28px | 22px | Section headings |
| H3 | Inter | 600 | 20px | 18px | Card titles, subsections |
| H4 | Inter | 600 | 16px | 15px | UI panel headers, labels |
| Body large | Inter | 400 | 18px | 16px | Marketing copy, introductory paragraphs |
| Body | Inter | 400 | 15–16px | 14px | General body text, descriptions |
| Body small | Inter | 400 | 13px | 12px | Supporting metadata, captions |
| Label / UI | Inter | 500 | 12–13px | 12px | Button labels, form labels, tags |
| Ticker | IBM Plex Mono | 500 | 14–16px | 13px | Asset tickers (e.g. AAPL, BTC/USD) |
| Price / Data | IBM Plex Mono | 400–500 | 13–16px | 12–14px | Prices, percentages, volume, timestamps |

### Typography Rules

- **Hierarchy first.** Use Space Grotesk only for display and H1/H2. Drop to Inter for H3 and below to maintain clear hierarchy.
- **Never use more than two fonts in a single component** — typically Inter + IBM Plex Mono (e.g. an alert card with a description in Inter and the price/ticker in IBM Plex Mono).
- **Line height:** 1.4–1.5× for body text. 1.1–1.2× for display/hero headings.
- **Letter spacing:** Slightly tightened (`-0.01em` to `-0.02em`) for large display text. Normal or slightly open (`0.01em`) for labels and small caps.
- **Colour on dark backgrounds:** Primary text in `#FFFFFF`, secondary/supporting in `#A0A0B8`.
- **Accent text:** Emerald `#00D68F` for positive highlights or key data points. Blue `#2979FF` for links and interactive elements. Never use accent colours for long-form body text.

---

## 3. Logo

### Assets

| File | Usage |
|------|-------|
| `Brand Assets/StockSight Logo.jpeg` | Icon mark only — favicons, app icons, watermarks |
| `Brand Assets/StockSight Logo with name.jpeg` | Standard logo — headers, documents, slide decks |
| `Brand Assets/StockSight Logo with slogan.jpeg` | Full brand mark — splash screens, marketing materials |

### Logo Rules

- Do not recolour or alter the logo mark
- Minimum clear space: equal to the height of the "S" mark on all sides
- Preferred placement on dark backgrounds only — do not place on light or coloured backgrounds without approval
- Watermark/corner usage: place at reduced opacity (≈ 60–70%) in bottom-right or bottom-left of image compositions

---

## 4. Voice & Tone Summary

- **Intelligent, confident, minimal.** Short sentences. Active voice.
- **Never:** financial advice framing, profit guarantees, competitor comparisons, slang, emojis in body copy
- **Taglines in active use:**
  - *"See the signal before the move."* — primary positioning line
  - *"Understand what's moving markets — instantly."* — product descriptor tagline

---

## 5. Reference

Full company positioning and messaging guidelines: `Brand Assets/StockSight AI - Company Overview.md`

Skills and content generation guidelines: `.claude/skills/create-ad/brand-guidelines.md`
