# Irisa's Archives

A personal library for your books, CDs, tapes, vinyl and films, with a shop mode that tells you whether you already own something before you buy it.

## Put it on GitHub Pages (about 5 minutes)

1. Sign in at github.com and click **New repository**. Name it `media-library` (or anything), set it to **Public** (free GitHub Pages needs public), and create it.
2. Click **uploading an existing file**, drag in **every file from this folder** (`index.html`, `sw.js`, `manifest.webmanifest`, `icon.svg`, `icon-180.png`, `icon-192.png`, `icon-512.png`), and commit.
3. Go to **Settings > Pages**. Under "Build and deployment", choose **Deploy from a branch**, pick `main` and `/ (root)`, and save.
4. After a minute your app is live at `https://YOURUSERNAME.github.io/media-library/`. That is your one address. Use it on your phone and computer.

Your collection is **not** stored in that public repo. It lives in your browser on each device.

## Install on your phone

Open your address in Safari (iPhone) or Chrome (Android), then **Add to Home Screen**. It opens like an app and works offline. Use the installed icon every time so you are always in the same library.

## Back up (important)

Your library is stored in your browser, so clearing site data would erase it. Under **More**:

- **Download backup** saves a `.json` file. **Load backup file** brings it back on any device.
- **Back up to GitHub** saves the library into a **private** repo:
  1. Create a second repo, set to **Private**, e.g. `my-library-data`.
  2. GitHub > Settings > Developer settings > Personal access tokens > **Fine-grained tokens** > Generate. Limit it to only that private repo, with **Contents: Read and write**.
  3. Enter your username, repo name and token under More > Back up to GitHub, then tap **Back up now**. On a new device, enter the same details and tap **Restore**.

The app reminds you if your last backup is older than two weeks.

## Scanning

- **Phone camera:** Shop > Scan barcode (needs the https address above).
- **USB or Bluetooth scanner:** just scan while the app is open. It reads the barcode like a keyboard. In Shop it runs the check immediately.
- **Typing:** enter a title, artist, or barcode number.

Details come from free public databases (Open Library, MusicBrainz, iTunes, a UPC lookup). Coverage is best for books and music; some films and obscure pressings will not be found and can be added by hand. Your own shelf check always works offline.

## Updating the app later

If you upload changed files, edit `VERSION` in `sw.js` (for example `irisa-v3`) so phones pick up the new version.
