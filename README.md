# Fortnite OG — Fan-made prototype

A responsive, original battle-royale-inspired web prototype. This is **not** an official Fortnite product and does not use Epic Games assets, sounds, skins, or branding beyond the project name requested for this prototype.

## Run it
Open `index.html` in a modern browser, or serve this folder with any static web server. No build step required.

## Included
- Responsive lobby and mobile/PC platform selection
- Local save system using `localStorage`
- Demo match simulation: eliminations award 1 coin, victory awards 30
- Shop with fictional original cosmetics and coin purchases
- Season timeline, event cards, loadout, bot-fill and platform-only matchmaking simulation
- Original synthesized UI sounds (Web Audio; no copyrighted audio files)

## Important limits
This is a front-end demo. It does not implement real multiplayer networking, authoritative anti-cheat, real 100-player servers, actual Fortnite maps/weapons/items, Epic account login, or real-money/V-Bucks transactions. The "V-Bucks" display is a mock counter only. Never enter payment or account credentials. A production game needs a backend, security review, legal review, and licensed assets.

## Project structure
- `index.html` — app shell
- `css/` — responsive styling split into modules
- `js/` — state, UI, shop, matchmaking, demo match, sound
- `assets/` — original SVG placeholders and manifest


## Render deployment
See `RENDER_DEPLOY.md`. Recommended: Render Static Site with Publish Directory `.` or deploy using the included `render.yaml` Blueprint. A Node Web Service alternative is available via `server.js` and `npm start`.
