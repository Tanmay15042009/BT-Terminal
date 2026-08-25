# BT Logger — GitHub Pages deploy

## Folder contents
- `index.html` — the app (with manifest link + service worker registration added)
- `manifest.json` — PWA manifest
- `service-worker.js` — offline caching
- `icons/` — app icons generated from your logo (16, 32, 180, 192, 512, and a maskable 512)
- `_headers` — Cloudflare Pages header rules (ignored by GitHub Pages, harmless to leave)
- `netlify.toml` — Netlify header rules (ignored by GitHub Pages, harmless to leave)

## Deploy on GitHub Pages
1. Go to https://github.com/new and create a new repository (public, any name — e.g. `bt-logger`). No need to initialize with a README.
2. On the new repo's page, click "uploading an existing file" (or drag files onto the page).
3. Upload everything in this folder, keeping the `icons/` folder structure intact.
4. Commit the upload.
5. Go to the repo's **Settings → Pages**.
6. Under "Build and deployment" → "Source", select **"Deploy from a branch"**.
7. Under "Branch", select **main** (or whichever branch you uploaded to) and folder **/ (root)**, then Save.
8. Wait ~1 minute — GitHub will give you a live URL like `https://yourusername.github.io/bt-logger/`.

No badge, no login wall, fully public and free.

## Installing on your phone
Once it's live:
- **Android (Chrome):** open the URL → menu (⋮) → "Install app" / "Add to Home screen".
- **iOS (Safari):** open the URL → Share → "Add to Home Screen".

## Going fully offline (APK route)
Once the GitHub Pages URL is live, paste it into https://pwabuilder.com to generate an installable `.apk`. Install that on your phone (one-time toggle: "allow install from this source"). After that, the app runs completely offline — you can delete the GitHub repo afterward and the APK keeps working.
