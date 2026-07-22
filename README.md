# Undertone — GitHub Pages + APK setup

## 1. Publish to GitHub Pages
1. Create a new GitHub repo (public).
2. Upload **all files in this folder** (`index.html`, `manifest.json`, `icon-512.png`, `styles.css`, `support.js`) to the repo root — keep them all at the top level, next to each other.
3. Repo → Settings → Pages → Source: "Deploy from branch" → branch `main`, folder `/ (root)` → Save.
4. Wait ~1 minute. Your live URL will be `https://<your-username>.github.io/<repo-name>/`.

## 2. Turn it into an APK with PWABuilder
1. Go to https://www.pwabuilder.com
2. Paste your GitHub Pages URL and click "Start".
3. PWABuilder scans the page's manifest/icon automatically (already embedded in this file) and shows a readiness report.
4. Click "Package for stores" → choose **Android** → download the generated package.
5. You'll get a signed `.apk` (or `.aab` for Play Store) — install the `.apk` directly on an Android phone (enable "install unknown apps" if prompted), or upload the `.aab` to Google Play Console to publish it.

That's it — no coding required beyond the upload.
