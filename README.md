# DollarTracker Stable v3

Local-only mobile ledger app.

## Important fixes

- Balance loads from storage immediately on first open.
- USD/KHR choice stays saved after refresh/app close.
- Copy button has 3 layers:
  1. Clipboard API
  2. iOS textarea fallback
  3. Manual prompt fallback
- Clear All Records uses a tap-twice system, not browser confirm.
- Records migrate from older Wifey Money/DollarTracker storage keys.
- Service worker now uses network-first for app files to reduce stale cache bugs.
- Flag paths are PNG:
  - `assets/flag-en.png`
  - `assets/flag-kh.png`

## Upload these files

- index.html
- styles.css
- app.js
- manifest.webmanifest
- service-worker.js
- icon.svg
- assets/flag-en.png
- assets/flag-kh.png
- README.md

## If iPhone still shows old behavior

It means iOS is still running old cached JavaScript. Delete the Home Screen app and clear the website data for the GitHub Pages domain, then open and add it again.
