# Set Clock

A workout set and rest timer for iPhone, built as an offline Progressive Web App.
No build step: `index.html` holds all the CSS and JS.

## Files

- `index.html` – the app
- `manifest.webmanifest` – name, colors and icons for Add to Home Screen
- `sw.js` – service worker that caches the app for offline use
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` – app icons
- `.nojekyll` – serves the files as-is on GitHub Pages

## Install on iPhone

1. Open the GitHub Pages URL in Safari.
2. Share → Add to Home Screen.
3. Open it once from the home screen while online; after that it works offline.

Workout history is stored in the browser's localStorage on the phone.

## Updating

After changing any file, bump `CACHE` in `sw.js` (e.g. `setclock-v3` → `setclock-v4`)
so installed copies fetch the new version.
