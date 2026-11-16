# EV Ledger – BYD Expense Tracker (PWA)

Track charging (units, rate, total), maintenance, body wash and other costs for your BYD,
with monthly charts and running cost per km. Installs on your phone and works offline.

## Files

```
index.html               the app
manifest.webmanifest     PWA manifest (name, icons, colours)
sw.js                    service worker (offline cache)
icons/                   app icons (192, 512, maskable, Apple touch)
img/                     model photos (Dolphin, Atto 1/2/3, Seal)
```

## Publish on GitHub Pages

1. Create a new **public** repository on github.com (e.g. `ev-ledger`).
2. **Add file → Upload files**, drag in everything from this folder
   (keep the `icons` and `img` folders), then **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment* choose
   **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After a minute your app is live at
   `https://<your-username>.github.io/ev-ledger/`

## Install on your phone

- **Android (Chrome):** open the link — an *Install EV Ledger* banner appears. Tap **Install**.
- **iPhone (Safari):** open the link, tap **Share → Add to Home Screen**.

## Your data

On GitHub Pages, all data is stored **on that device only** (browser storage).
Use **Backup** on the dashboard regularly to save a `.json` copy, and **Restore**
to move it to a new phone. Uninstalling the app or clearing browser data deletes it.

## Updating the app

When you upload changed files, open `sw.js` and bump `VERSION`
(e.g. `ev-ledger-v1` → `ev-ledger-v2`) so phones pick up the new version.
