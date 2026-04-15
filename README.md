# Ducote Consulting — New Site (GitHub Pages Ready)

A full rebuild of the Google Sites `ducoteconsultingclientsmap` property — all original content preserved, visuals restored, and the broken map overlay fixed.

## What's inside

```
site/
├── index.html         Home with hero, stats, services preview, service area, CTA
├── about.html         Company history, process, values
├── services.html      All 6 services + who-we-serve + engagement models
├── team.html          Nick, Sarah, Judy, Ian — full bios and photos
├── portfolio.html     Fixed, full-width interactive Google My Map + legend
├── assets/
│   ├── css/style.css  Brand palette, fully responsive, mobile nav
│   ├── js/main.js     Mobile menu, active nav, scroll reveal
│   └── img/           All original imagery (logos + hero + team photos)
└── README.md
```

## Brand palette (pulled directly from the original site)
| Token | Hex | Role |
|-------|-----|------|
| `--ink` | `#131211` | Sidebar / dark sections |
| `--ink-2` | `#1C1C1C` | Dark neutral |
| `--orange` | `#BF6430` | Primary accent — burnt orange |
| `--teal` | `#3B7D8C` | Secondary accent |
| `--cream` | `#E6E3DF` | Page background |
| `--paper` | `#F9F9F9` | Card / light section |

Typography: **Cormorant Garamond** (display serif) + **Inter** (body sans).

## Map fix

The original Google Site embedded the Clients Map at a wrong size which clipped the overlay. The rebuild uses:

- Proper `iframe` with `mid=1jUhXKQAMCi--rMUHzzcnVUpSYHwnGa0`
- Fluid full-width container with `height:78vh` on desktop / `60vh` on mobile
- "Open full map in new tab" button for the complete MyMaps experience
- Legend block below explaining pin categories

## Deploy to GitHub Pages

1. Create a new GitHub repo (e.g. `ducote-site`).
2. Copy the contents of `site/` to the repo root.
3. Push to `main`.
4. In the repo settings → Pages → source = `main` / `/ (root)`.
5. Your site goes live at `https://<user>.github.io/ducote-site/`.

Alternative: push `site/` contents to the `gh-pages` branch.

## Source archives

- `raw/*.html` — original HTML for each page
- `raw/*-rendered.html` — full DOM after JS execution
- `raw/*-screenshot.png` — visual snapshots of the original site
- `content/*.md` — verbatim text content extracted from each page
- `images/` — all source imagery (originals + fallbacks)
