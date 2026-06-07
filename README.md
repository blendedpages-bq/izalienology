# Izalienology

Static site for [izalienology.com](https://izalienology.com) — the living codex of the BlendedPages creative universe.

Deployed via Cloudflare Pages.

---

## File Structure

```
izalienology/
  index.html                        ← Homepage (live)
  thecodex/
    index.html                      ← The Codex page (pending)
  voices/
    index.html                      ← Voices page (pending)
  the-future-is-watching/
    index.html                      ← The Future is Watching page (pending)
  assets/
    images/
      web-background.webp           ← Hero background
      khael-web.webp                ← Khael Vireon portrait
      sirae-web.webp                ← Sirae Ilyon portrait
      house-veran-sigil-907x907.webp ← Covenant flame / First Hearth
      hallofbanners.webp            ← Hall of Banners full-width image
      favicon-izalienology-steal-blue-ring-32x32.webp
```

---

## Design System

- **Fonts:** Cinzel (headings) · Cormorant Garamond (lore) · Jost (UI)
- **Base:** `html { font-size: 62.5% }` — all sizing in rem
- **Breakpoint:** 900px — 2-col collapses to 1-col
- **Colors:**
  - `#06050f` — void (base background)
  - `#c9922a` — covenant gold (primary accent)
  - `#e8b84b` — gold light (highlights)
  - `#dddbe8` — silver (primary text)
  - `#9290a8` — silver dim (secondary text)

---

## Build Notes

- Pure HTML/CSS — no frameworks, no build step
- No JavaScript
- No external dependencies except Google Fonts
- Images: all `.webp`, served from `assets/images/`
- Cloudflare Pages deployment: push to `main` branch → auto-deploys

---

## Roadmap

- [x] `index.html` — Founders, Six Houses teaser, locked
- [ ] `thecodex/index.html` — Uses `codexcavern.webp` + `izalien.mp4`
- [ ] `voices/index.html` — Manuscript voice quotes
- [ ] `the-future-is-watching/index.html` — Pre-covenant teaser
- [ ] Email capture — add when book nears completion
- [ ] Six Houses unlock — Book II launch

---

## Part of the BlendedPages Universe

**Book I: Izalienology** — *Forged in Pain* — B. Patrick Bradley  
Published by BlendedPages · Sheridan, WY  
© 2025 BlendedPages. All rights reserved.
