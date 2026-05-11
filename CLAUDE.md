# Inner Worth Wellness — Project Rules

## What this project is

Single-page static website for **The Inner Worth Wellness** (Dr. Garvita Vyas), Vadodara, India.

**Tech stack:** Vanilla HTML/CSS/JS · Tailwind CDN · Lucide CDN · Google Fonts (Instrument Serif + Inter Tight)

**File structure:**
- `index.html` — full single-page site, all sections in one file
- `assets/hero-bg.png` — hero background (Ken Burns animated)
- `assets/logo-lotus.png` — official logo used in nav and footer
- `docs/garvita-sessions-guide.html` — guide doc for Garvita (local only, not committed)

**Design tokens:**
- Background: `#ece4d6` (warm cream)
- Primary/CTA: `#2a3a26` (moss green)
- Accent: `#c47a78` (rose)
- Fonts: Instrument Serif (headings) + Inter Tight (body)

**Wired contacts:**
- Calendly: `https://calendly.com/theinnerworthwellness/30min`
- WhatsApp: `+919173243337`
- Email: `hello@innerworth.co`
- Instagram: `https://www.instagram.com/theinnerworthwellness/`

---

## Git rules

**Only commit files that ship to the site.** Nothing else.

Files that belong in git:
- `index.html`
- `assets/` (images, fonts)

Files that must NOT be committed:
- `docs/` — guide docs for Garvita, local only
- `docs/superpowers/` — plans and specs, local only
- `.claude/` settings

When staging, always use explicit file paths (`git add index.html assets/...`). Never `git add .` or `git add -A`.

---

## Code rules

- No frameworks, no build steps — keep it vanilla HTML/CSS/JS
- No new files unless explicitly required
- All JS lives in `index.html` in the `<script>` block at the bottom
- All CSS lives in `index.html` in the `<style>` block in `<head>`
- Do not split into separate `.js` or `.css` files
