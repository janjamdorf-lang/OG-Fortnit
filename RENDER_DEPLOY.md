# Fortnite OG — Render Deployment

This repository is configured for **Render Static Site**, which is the simplest and recommended way to publish this browser prototype.

## Option A — Render Blueprint (recommended)

1. Put the contents of this folder in a GitHub repository.
2. Sign in to Render.
3. Choose **New + → Blueprint**.
4. Connect the repository and select `render.yaml`.
5. Confirm the service creation. Render will publish the static files and provide a public `onrender.com` URL.

The Blueprint sets `staticPublishPath: .` because `index.html` and the `css/`, `js/`, and `assets/` folders live at the repository root.

## Option B — Create a Static Site manually

In Render choose **New + → Static Site**, connect the repository, then use:
- **Build Command:** leave empty
- **Publish Directory:** `.`

Deploy the site. No build step or package installation is needed for the static site.

## Option C — Node Web Service

If you specifically want a Render **Web Service**, select Node as the runtime and set:
- **Build Command:** `npm install`
- **Start Command:** `npm start`

The included `server.js` serves the files on `process.env.PORT`. For this front-end prototype, a Static Site is cheaper and simpler.

## Important

- This is a fan-made prototype, not an official Fortnite product.
- Local progress is stored in each browser's `localStorage`. It does not sync between devices and may be cleared with browser data.
- The match and bots are simulations, not online multiplayer.
- Do not add payment details or Epic account credentials. Real accounts, secure persistence, real matchmaking, and actual multiplayer require a separate backend and security work.
- Only upload art, music, and sound assets you own or have permission to use.
