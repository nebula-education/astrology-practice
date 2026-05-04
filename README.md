# Mini Chart Reading — Practical Module

A two-track interactive astrology lesson for Nebula Academy.

- **Track A — Relationships**: Sun · Moon · Venus · Ascendant
- **Track B — Career**: Sun · Moon · Midheaven · Ascendant

## Structure
- `index.html` — single-file module (CSS + JS inlined)
- `astronomy.min.js` — cosinekitty/astronomy-engine v2.1.19, used by the live chart calculator
- `images/` — chart wheel zooms and brand celestials (inline SVGs)

## Key interactions
- **Pick a track** on the hero (Relationships / Career card)
- **Click any chart image** in a step — the reading reveals beneath
- **Self-practice prompts** under every reading
- **Sticky track switcher** lets the learner jump between tracks
- **Floating fullscreen button** (bottom-right) — stakeholder requirement

## Build Your Own Chart (interactive calculator)
After the three guided steps, learners can compute a real natal chart from
their own birth data:

- Birth date, time, city (15 presets + custom lat/lon)
- Whole Sign or Placidus house systems
- Toggleable major aspects (Conjunction · Sextile · Square · Trine · Opposition)
- Optional **transit overlay** for any chosen date

The engine uses VSOP87/ELP-2000 ephemerides via astronomy-engine and was
validated against Rodden AA reference charts — Princess Diana's chart matches
astro.com's Placidus output to within 1 arcminute on Sun, Moon, ASC, MC.

## Deploy
Drop the folder into a GitHub repo and enable Pages — no build step needed.
Both files (`index.html` and `astronomy.min.js`) must sit in the same folder.
