# Uge Press — Visual Identity Guide

*This is the single source of truth for how Uge Press looks and sounds. Every decision here was made once so it never has to be made again.*

---

## 01. The Mark

### Primary Logo (Concept 1 — Recommended)
The Uge Press logo consists of two elements: the **wave mark** and the **wordmark**.

- **Wave mark:** A single, clean Bézier curve — thin at origin, swelling slightly at crest, tapering to a fine point. It references Brooke's wave symbol without literalizing it. It is architectural, not decorative.
- **Wordmark:** "UGE · PRESS" — "UGE" in Cormorant Garamond, "PRESS" in Inter Light, separated by a centered dot or em-space. Wide letter-spacing throughout.

The wave mark should always appear to the left of the wordmark, vertically aligned to the cap-height midpoint of "U."

### Icon / Favicon
The wave mark alone, in Terracotta on Cream background. No wordmark. Used at 32×32px and smaller.

### Clear Space
Maintain clear space equal to the height of the capital "U" on all four sides of the logo. No competing elements, borders, or patterns within this zone.

### Minimum Size
- **With wordmark:** 140px wide (digital) / 1.5 inches wide (print)
- **Icon only:** 16px (digital) / 0.25 inches (print)

### Prohibited Uses
- Do not recolor the logo outside the approved palette
- Do not stretch, rotate, or apply drop shadows
- Do not use on busy photographic backgrounds without a clear field
- Do not use a bold or condensed weight for the wordmark
- Do not use the wave mark as a decorative element separate from the brand system

---

## 02. Color Palette

### Primary Colors

| Name | Hex | Use |
|------|-----|-----|
| Cream | `#FAF8F5` | Background, reversed logo field |
| Charcoal | `#1a1a1a` | Primary type, logo wordmark |
| Terracotta | `#C45D3E` | Accent, wave mark, CTAs, rule lines |

### Secondary Colors

| Name | Hex | Use |
|------|-----|-----|
| Warm Grey | `#4a4a4a` | Body text, secondary headings |
| Light Grey | `#8a8a8a` | Captions, taglines, metadata |
| Soft Border | `#e8e4df` | Dividers, borders, hairlines |
| White | `#FFFFFF` | Card backgrounds, quote boxes |

### Usage Principles
- **Cream is the ground.** The website, stationery, and most print materials live on cream. White is a deliberate lift — for cards, callout boxes, things that need to float.
- **Terracotta is the accent, not the brand.** It appears once per composition — a rule, a button, the wave mark, a border. Not multiple times. It's a signature, not wallpaper.
- **Charcoal, not black.** `#1a1a1a` is warmer than pure black. It matches the warmth of the cream background and creates a softer, more editorial contrast.

### Dark Mode / Reversed
- Swap: Charcoal background, Cream type
- Wave mark: Terracotta (unchanged)
- Use reversed palette for email headers, book spines, social profile banners

---

## 03. Typography

### Type System

| Role | Font | Weight | Size | Notes |
|------|------|--------|------|-------|
| Display / Hero | Cormorant Garamond | 400 (Regular) | 42–60px | Never bold for display |
| Section Headings | Cormorant Garamond | 400 | 28–36px | Italic variant for pull quotes |
| Sub-headings | Inter | 500 (Medium) | 17–20px | Sentence case, not all-caps |
| Body Copy | Inter | 300 (Light) | 16–18px | Line height 1.7 |
| Captions / Meta | Inter | 300 | 13–14px | Letter-spacing +0.5px |
| Logo / Label | Cormorant Garamond | 400 + Inter 300 | — | See logo specs above |

### Typography Rules

1. **Cormorant for feel. Inter for function.** Cormorant headings create the editorial warmth. Inter body copy ensures readability. Do not mix roles.

2. **Never bold Cormorant in running text.** Bold Cormorant reads as shouting. For emphasis within Cormorant, use italic. For emphasis within Inter, use 500 weight.

3. **Wide tracking on all-caps text.** If you set something in all-caps (labels, section markers, the word PRESS), track it out: minimum +80, ideally +120–200. Untracked all-caps looks like a URL, not a publisher.

4. **Let the type breathe.** Line height 1.7 for body text. Section headings: 1.2–1.3. Margins between sections: never less than 48px on desktop.

5. **Hierarchy through contrast, not size.** The difference between a Cormorant 36px heading and Inter 17px body is enormous. Don't compensate by making headings 60px. Restraint is sophistication.

---

## 04. Website Design Enhancements

*The current site (ugepress.com) is good. These suggestions elevate it.*

### Logo Placement
- Replace the current text-only `.logo` div with the SVG logo mark (wave + wordmark)
- Size: wave mark at ~40px height, wordmark at ~22px — matches current visual weight exactly
- Left-aligned, same position — no change to layout

### Header Refinement
- Reduce header padding from `60px 0 40px` to `48px 0 32px` — slightly more compact, more editorial
- Add a `letter-spacing: 0.5px` to the tagline — it currently reads a little flat
- Consider replacing the bottom border hairline (`#e8e4df`) with a Terracotta rule, 1px — one thin accent line that establishes the color story before any other element appears

### Hero Section
- The `h1` at 48px is excellent. Keep it.
- The `.hero p` at 19px is slightly large. Reduce to 18px — more editorial, less landing-page.
- Add `font-style: italic` to the `.hero .quiet` caption — it's set in Inter right now, which works, but italic Inter 300 reads more like a genuine whisper

### Quote Box
- Currently: `border-left: 3px solid var(--warm-accent)` — this is the right instinct
- Refinement: change `border-left` width from 3px to 2px — thinner is more refined at this price point
- Increase left padding from 28px to 32px — the quote needs more air between the rule and the first word

### Process Steps
- The step numbers in Terracotta are strong — keep them
- Consider adding `font-style: italic` to the step numbers — makes them more expressive, less "listicle"
- Add subtle `opacity: 0.7` to step numbers when not the first step — draws the eye naturally down the sequence

### Pricing Section
- The white card with border is clean — keep it
- Add `border-top: 2px solid var(--warm-accent)` to `.pricing-note` — a single horizontal accent at the top of the card, instead of a full border — this is how editorial publications style feature boxes

### CTA Section
- The `.cta-button` in full Terracotta is correct
- Refine: increase letter-spacing from wherever it is now to `2px` — uppercase tracking on a premium CTA should be generous
- Add `:hover` state: `background: #a84d31` (a 10% darker Terracotta) + `letter-spacing: 2.5px` for a barely-perceptible bloom effect

### Footer
- If there isn't one: add a minimal footer — single line, centered
- "© 2026 Uge Press" in Inter 300, 13px, Light Grey
- A thin horizontal rule above it, full width, `#e8e4df`
- Nothing else. Publishers don't need cluttered footers.

### Spacing System
Adopt an 8px base grid. Every vertical spacing decision should be a multiple of 8: 8, 16, 24, 32, 40, 48, 64, 80, 96. The current site is close — formalize it.

---

## 05. Brand Voice

*The visual identity and the verbal identity are one thing.*

### Tone
**Restrained confidence.** We know what we're doing. We don't need to prove it. We don't use exclamation points. We don't say "amazing" or "incredible." We let the work speak.

### Voice Qualities
- **Precise:** Specific words, not general ones. "We preserve your voice" not "we make your writing better."
- **Warm:** Professional without being corporate. An editor's warmth, not a consultant's warmth.
- **Direct:** Short sentences. Active voice. No throat-clearing.
- **Literary:** We are a publishing house. Our copy should read like it was written by someone who edits books for a living.

### Words We Use
honest · precise · craft · voice · concierge · editorial · considered · deliberate · transformation · partnership

### Words We Avoid
amazing · incredible · revolutionary · cutting-edge · seamless · leverage · synergy · solutions · AI-powered (use sparingly, explain honestly)

### Punctuation Style
- Em dash over parentheses, used sparingly
- Oxford comma, always
- No ellipses in formal copy
- Italics for titles, emphasis — not quotation marks

### The Test
Read it aloud. Does it sound like a brilliant editor wrote it, or like a startup wrote it? If the latter: cut half the words and start again.

---

## 06. Application Examples

### Email Signature
```
Brooke Grace
Editor, Uge Press
ugepress.com
```
*No phone number unless requested. No logos in email signatures — the name is enough.*

### Social Profile Bio
```
Boutique nonfiction editing. 7 days. $2,000. No slop.
ugepress.com
```

### Document Header (Editorial Reports)
- Uge Press logo mark, top-left
- Client name + manuscript title, right-aligned, Inter 300
- Terracotta hairline rule beneath header, full width
- Everything below: Charcoal on white, Inter 300, 12pt, 1.6 line height

---

*This guide was written April 2026. It will evolve as the brand does. The principles will not.*

— Brooke Grace, Uge Press
