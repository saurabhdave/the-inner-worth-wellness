# FAQ & Myths — Design Spec
_Inner Worth Wellness · 2026-05-10_

## Overview

Add two new sections to `index.html`:
1. **Myths & Myth Busters** — addresses misconceptions about the modalities to reduce hesitation
2. **FAQs** — answers practical questions for clients close to booking

---

## Section 1: Myths & Myth Busters

### Placement
Between the existing **Modalities** section and the **About** section.

### Anchor
`id="myths"`

### Layout & Styling
- Background: `#ece4d6` (same warm cream as the page)
- Padding: `px-6 md:px-10 lg:px-20 py-24 md:py-32` (matches existing sections)
- Soft aurora background effect (same `.soft-aurora` class used in Modalities)
- Section badge: "Setting the record straight" with sparkles icon
- Headline: `"What healing is not."` — serif, italic accent on "not", same size as other section headlines (`text-4xl md:text-5xl lg:text-[64px]`)
- Subtitle: `"The most common worries — and the truth behind them."`

### Card Grid
- `grid-cols-1 md:grid-cols-2 lg:grid-cols-3` with `gap-5 md:gap-6`
- 6 cards total, each using `.iv` scroll-reveal class
- Card base: `bg-[#f4ecdb] rounded-[1.8rem] p-7 border border-[#3a322a]/8`
- Hover lift: `.modality` class (same as modality cards)

### Card Anatomy (each card)
1. **Modality tag** — small pill in top-left:
   - Hypnotherapy: `bg-[#2a3a26] text-[#f5ecd9]`
   - Sound Therapy: `bg-[#9aa988] text-[#2a241e]`
   - Inner Child: `bg-[#e9d5c4] text-[#5a3024]`
2. **Myth text** — serif, `text-[18px]`, `text-[#a08878]`, `line-through` decoration, italic
3. **Divider row** — thin line, rose `→` arrow centre, thin line
4. **Truth text** — `text-[14px]`, `text-[#2a3a26]`, `font-medium`, `leading-relaxed`

### The 6 Myths (in order)
| # | Tag | Myth | Truth |
|---|-----|------|-------|
| 1 | Hypnotherapy | "You lose control — I can make you do anything." | You remain fully aware and in control throughout every session. |
| 2 | Hypnotherapy | "It puts you to sleep and you won't remember." | You're in a relaxed but alert state — aware of everything. |
| 3 | Hypnotherapy | "Only weak-minded people can be hypnotised." | Responsiveness reflects focus and creativity, not weakness. |
| 4 | Hypnotherapy | "It implants false memories or suggestions." | Sessions are guided by your own inner landscape — nothing is imposed. |
| 5 | Sound Therapy | "It's just relaxing background music." | Frequencies create measurable brainwave and nervous system shifts — it's physics, not ambience. |
| 6 | Inner Child | "This is only for people with serious trauma." | Anyone who learned to people-please, over-perform, or shut down emotions benefits. |

---

## Section 2: FAQs

### Placement
Between the existing **Testimonials** section and the **CTA (Begin)** section.

### Anchor
`id="faq"`

### Layout & Styling
- Background: `bg-[#f4ecdb]` (warm off-white, same as About and Journey sections)
- Padding: `px-6 md:px-10 lg:px-20 py-24 md:py-32`
- Section badge: "Common questions" with a `help-circle` icon
- Headline: `"Before you reach out."` — serif, italic accent on "reach out"
- No subtitle needed — the cards are self-explanatory

### Card Grid
- `grid-cols-1 md:grid-cols-2 lg:grid-cols-3` with `gap-5 md:gap-6`
- 6 cards total, each using `.iv` scroll-reveal class
- Card 2 uses dark moss treatment (`bg-[#2a3a26] text-[#f5ecd9]`) for visual rhythm — same alternating pattern as Testimonials

### Card Anatomy (each card)
1. **Number** — serif, `text-[48px]`, `leading-none`, `text-[#3a322a]/15` (light, decorative)
2. **Question** — `text-[16px]`, `font-medium`, `text-[#2a241e]`, `leading-snug`
3. **Answer** — `text-[14px]`, `text-[#5a4d40]`, `leading-relaxed`
   - Dark card variant: number `text-[#f5ecd9]/15`, question `text-[#f5ecd9]`, answer `text-[#f5ecd9]/75`

### The 6 FAQs (in order)
| # | Style | Question | Answer |
|---|-------|----------|--------|
| 1 | Light | Do I need any prior experience with these therapies? | None at all. Sessions are shaped around wherever you are — first-timers are always welcome. Garvita takes time to understand your context before anything begins. |
| 2 | **Dark** | How many sessions will I need? | Most people notice a meaningful shift within 1–3 sessions. Deeper work — habit change, grief, regression — often unfolds over 6–8. There's no fixed prescription; we reassess together as you progress. |
| 3 | Light | Are sessions available online? | Yes. Sound therapy, hypnotherapy, and inner-child work all translate well to an online setting. In-person sessions are available at the Vadodara studio. |
| 4 | Light | Can I combine modalities in a single session? | Yes — Garvita often weaves sound and hypnotherapy, or sound and inner-child work, depending on what you're carrying. The session is always shaped around you, not a fixed protocol. |
| 5 | Light | What should I bring or wear? | Wear something you can lie down and breathe in comfortably. For in-person sessions, bring a light blanket or shawl. Nothing else is needed — just yourself. |
| 6 | Light | What if I've tried therapy before and it didn't help? | Many clients come after years of talk therapy. These modalities work through the body and the subconscious — they reach places words sometimes don't. We always start gently. |

---

## Navigation

Add `"FAQ"` as a nav link to the desktop menu, pointing to `#faq`. Insert between "Stories" and "Journey" in the existing list.

---

## .gitignore Update

Add `.superpowers/` to `.gitignore` (brainstorming session files should not be committed).

---

## Files Changed

- `index.html` — add Myths and FAQ sections, update nav
- `.gitignore` — add `.superpowers/`
