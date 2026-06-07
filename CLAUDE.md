# CLAUDE.md — izalienology.com Brand Data
 
## Project Overview
**Site:** izalienology.com
**Role in universe:** Mythic lore foundation — the deepest layer of the BlendedPages creative universe
**Tagline:** "From one covenant, six legacies will rise."
**Status:** Static HTML placeholder, deployed to Cloudflare Pages (free tier)
**Migration deadline:** June 11, 2025 (migrating off SiteGround hosting)
**Built:** June 2025
 
---
 
## Universe Hierarchy
```
BlendedPages (blendedpages.com) — parent brand/universe
  └── Izalienology (izalienology.com) — mythic lore foundation / living codex
        └── Izaliens (izaliens.com) — teen sci-fi series (the Houses reborn)
              └── Glowheart Station — children's series (forthcoming)
```
 
---
 
## Brand Identity
 
### Tone & Aesthetic
- **Tone:** Mythic, cosmic, ancient-feeling but sci-fi. Epic fantasy meets space opera.
- **Aesthetic:** Dark, dramatic, monumental. NOT corporate. NOT children's brand. Epic literary sci-fi.
- **Energy:** Deep space / ancient covenant. Like carved stone glyphs in zero gravity.
- **This site is:** The lore foundation — the codex, the origin story, the world-building layer everything else rests on.
### Brand Voice
- Mythic, weighty, literary
- Present tense for the living codex; past tense for the covenant origin
- Contradiction is intentional — different Houses interpret the same events differently
- Sentences that earn their gravity; no inflation
---
 
## Color System
 
| Variable | Value | Use |
|---|---|---|
| `--color-void` | `#04030a` | Base background, near-black deep space |
| `--color-deep-space` | `#080714` | Section background variation |
| `--color-abyss` | `#0d0b1e` | Card/panel backgrounds |
| `--color-indigo-dark` | `#12103a` | Subtle panel variation |
| `--color-gold` | `#c9922a` | Covenant gold — primary accent, section labels |
| `--color-gold-light` | `#e8b84b` | Highlights, hover states, hero heading accent |
| `--color-gold-dim` | `#7a5518` | Borders, muted gold, divider lines |
| `--color-silver` | `#e2e0ee` | Primary body text |
| `--color-silver-dim` | `#9896b0` | Secondary text, captions, nav links |
| `--color-crimson` | `#8b1a2a` | Danger, sacrifice, depth accent (reserved) |
| `--color-crimson-glow` | `#b52238` | Crimson highlight (reserved) |
 
### House Colors
| House | Variable | Value | Meaning |
|---|---|---|---|
| Empathy | `--house-empathy` | `#7b4fa6` | Violet — compassion, feeling |
| Memory | `--house-memory` | `#2e7ab5` | Sapphire — deep knowing |
| Strength | `--house-strength` | `#c75b2a` | Ember — forged endurance |
| Unity | `--house-unity` | `#2e9e6e` | Viridian — bonds, growth |
| Justice | `--house-justice` | `#c9922a` | Gold — balance, covenant |
| Hope | `--house-hope` | `#4a9fb5` | Pale cerulean — horizon light |
 
---
 
## Typography
 
| Variable | Value | Role |
|---|---|---|
| `--font-heading` | `'Cinzel', serif` | All headings, logo, house names — Roman gravitas |
| `--font-sub` | `'Cormorant Garamond', serif` | Subheadings, body lore text, italics — elegant editorial |
| `--font-body` | `'Jost', sans-serif` | Nav, labels, utility text, captions — clean readable |
 
**Google Fonts import:** Cinzel (400–900), Cormorant Garamond (300–600 + italics), Jost (300–500)
 
---
 
## Layout System
- `html { font-size: 62.5%; }` → all sizing in rem
- `--max-width: 1200px` container, `margin: 0 auto`
- Responsive breakpoint: `≤900px` → all 2-col grids collapse to 1-col
- Secondary breakpoint: `≤600px` → Houses grid collapses to 1-col
- Navigation: sticky, `backdrop-filter: blur(12px)`, gold border-bottom
---
 
## Space System
| Variable | Value |
|---|---|
| `--space-xs` | `0.8rem` |
| `--space-sm` | `1.6rem` |
| `--space-md` | `3.2rem` |
| `--space-lg` | `6.4rem` |
| `--space-xl` | `9.6rem` |
| `--space-2xl` | `12.8rem` |
 
---
 
## Page Sections (index.html)
 
### 1. Navigation
- Sticky, dark (`rgba(4,3,10,0.88)`), backdrop blur
- Logo: "Izalienology" in Cinzel, gold-light
- Links: Covenant, Houses, Codex, Universe
- Hidden at ≤900px (mobile)
### 2. Hero
- Full viewport height minus nav
- Animated star field: CSS `radial-gradient` dots on `body::before`
- Nebula glow: CSS gradients on `body::after` (fixed, layered)
- SVG covenant glyph ornament (CSS-drawn, above heading)
- Animated entrance: `fadeUp` keyframes, staggered `animation-delay`
- Gold circle ring ornament behind heading via `::after` pseudo-element
### 3. The Covenant (`#covenant`)
- 2-column grid: text left, rotating SVG seal right
- Origin story: Khael Vireon & Sirae Ilyon
- Seal: SVG drawn hexagram + rings, CSS `sealRotate` animation (60s linear infinite)
### 4. The Six Houses (`#houses`)
- 3-column grid → 2-col at 900px → 1-col at 600px
- Each house card: dark panel, colored top border, glow on hover
- `--house-color` custom property per card for color theming
- Each has: SVG sigil icon, numeral (House I–VI), name, 2-sentence lore description
### 5. The Codex (`#codex`)
- Centered, max-width 840px
- Pull quote styled as `<blockquote>` with left gold border
- 3-paragraph explanation of what Izalienology IS
### 6. The Universe (`#universe`)
- 2-column grid of link cards
- BlendedPages (parent) and Izaliens (child series)
- Each card: labeled, titled, described, arrow CTA
### 7. Footer
- Logo repeat, tagline, gold rule
- Nav links to all sites and sections
- Copyright: © 2025 BlendedPages
---
 
## Key Lore Content
 
### The Founders
- **Khael Vireon** — keeper of flame and form; will to act, build, defend
- **Sirae Ilyon** — weaver of voice and memory; will to remember, honor, carry forward
### The Covenant
Not a ceremony — a declaration written into the structure of what would follow. The promise: that power without empathy is ruin, memory without justice is cruelty, strength alone cannot carry hope. The legacies will endure.
 
### The Six Houses (full descriptions)
1. **Empathy** — "To bear witness to another's pain as if it were your own — this is not weakness. It is the oldest form of power. The House of Empathy holds the covenant's first breath."
2. **Memory** — "History is not erased — it is remembered, wrestled with, and redeemed. The House of Memory carries every name of the fallen, every oath spoken into the void."
3. **Strength** — "Forged in the crucible of sacrifice, strength is not domination — it is the endurance to remain standing when every reason to fall has been given. They hold the line."
4. **Unity** — "No legacy survives in isolation. The House of Unity weaves the bonds between worlds, between peoples, between the inheritance of the past and the promise of what comes next."
5. **Justice** — "The covenant was not made to preserve comfort — it was made to correct what was broken. The House of Justice carries the flame of accountability across every generation."
6. **Hope** — "When the covenant seemed lost, when silence swallowed whole civilizations, the House of Hope was the signal that endured — the light at the edge of a dying galaxy that refused to go dark."
---
 
## Visual Techniques Used (no image dependencies)
 
| Element | Implementation |
|---|---|
| Star field | CSS `radial-gradient` dots on `body::before` (fixed position) |
| Nebula glow | CSS `radial-gradient` atmospheric overlay on `body::after` (fixed) |
| Covenant seal | Inline SVG — hexagram, rings, tick marks, CSS `sealRotate` animation |
| Hero glyph | Inline SVG — 6-pointed form with crossing lines |
| House sigils | Inline SVG — unique per house (heart, spiral, triangle, rings, scales, star) |
| Gold dividers | CSS gradient `linear-gradient` on `<span class="gold-rule">` |
| Card hover glow | CSS `radial-gradient` via `::after` pseudo-element, `opacity` transition |
| Hero circle ornament | CSS `::after` on `.hero`, border-radius 50%, box-shadow |
 
---
 
## Assets Directory
```
assets/
  images/    ← empty, ready for future imagery
```
 
**Future image slots to fill:**
- Hero background: deep space nebula photography (optional — CSS background works well)
- Covenant section: portrait art of Khael Vireon & Sirae Ilyon
- House cards: individual house banner/sigil artwork (per house)
- Codex section: codex/tome imagery
---
 
## Deployment
- **Host:** Cloudflare Pages (free tier)
- **Domain:** izalienology.com
- **Build:** Static — push index.html, no build step required
- **Connected sites:** blendedpages.com, izaliens.com
---
 
## Related Sites (same migration project)
| Site | Role | Status |
|---|---|---|
| blendedpages.com | Parent brand | ✅ Built |
| izaliens.com | Teen sci-fi series | ✅ Built |
| icarehomeloans.com | Mortgage platform | ✅ Built |
| izalienology.com | Lore foundation | ✅ Built |
| (remaining) | TBD | 🔲 Pending |
