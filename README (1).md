# PolyPulse 🎷📈

**The pulse of the prediction markets — with Market Mama on the mic.**

PolyPulse is a live trend tracker for [Polymarket](https://polymarket.com) prediction markets, built entirely with **vanilla HTML, CSS, and JavaScript** — no frameworks, no build step, no API key. Drop `index.html` on GitHub Pages and it runs.

## Features

- **Live market data** — pulls the hottest open markets straight from Polymarket's public Gamma API (`gamma-api.polymarket.com`), refreshed every 60 seconds
- **Marquee ticker** — a scrolling strip of top markets and live YES prices, jazz-club-meets-trading-floor style
- **Three lenses** — sort by 24h volume (hottest), ending soon, or true toss-ups (markets priced near 50¢)
- **Instant search** — filter every loaded market as you type
- **Probability bars** — YES/NO split visualized on every card, with prices shown in cents (67¢ YES = the crowd says 67% likely)
- **Installable app (PWA)** — includes a web manifest and service worker, so on phones you can tap "Add to Home Screen" and PolyPulse opens full-screen with its own icon, like a native app. The shell loads instantly from cache; prices always come live from the network.
- **Mama's Read (AI insight)** — an AI panel that summarizes what the crowd is betting on today, powered by Claude when the app runs inside a Claude artifact; gracefully degrades on the static site

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire app — markup, styles, and logic |
| `manifest.json` | PWA manifest (name, icons, theme) — makes the app installable |
| `sw.js` | Service worker — caches the shell, keeps market data live |
| `icon-192.png` / `icon-512.png` | App icons |
| `CONTRIBUTOR_AGREEMENT.md` | Ownership and contribution terms |

## Stack

| Layer | Choice |
|---|---|
| Markup | HTML5, semantic elements |
| Style | Hand-written CSS custom properties, grid, `prefers-reduced-motion` respected |
| Logic | Vanilla ES2020 JavaScript, `fetch`, zero dependencies |
| Data | Polymarket Gamma API (public, read-only, CORS-enabled) |
| Hosting | GitHub Pages |

## Run it

1. Clone the repo
2. Open `index.html` in a browser — that's it
3. To deploy: push to GitHub → Settings → Pages → serve from `main` branch root

## Notes

- Gamma API returns `outcomes` and `outcomePrices` as JSON *strings*, so the app parses them defensively (`parseMaybeJSON`)
- Prices ≈ implied probabilities: a YES share trading at 67¢ pays $1 if the event happens
- Not financial advice. Mama just reports what the crowd is doing.

## Creator

Created and led by **Aisha Hosley Abiola**. Started July 2026.

## Contributing

Contributions are welcome and credited in full — read [CONTRIBUTOR_AGREEMENT.md](CONTRIBUTOR_AGREEMENT.md) before submitting any changes.

## License

All rights reserved. No license is granted to copy, modify, or redistribute this code outside of an approved contribution under the Contributor Agreement.

---

*A Galsinger Media lab project.*
