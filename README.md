# Dishkeep — v4 (working brand)

Your private, photo-forward, offline-first cookbook. Install on iPhone via Safari → Share → Add to Home Screen.

## Included
- Modern compact photo cards, list/grid, dark mode and filters
- Collections, favorites and full-text offline search
- Recipe pages, ingredient checklists, one-step-at-a-time cooking mode
- Add recipes manually or through a review screen
- Import schema.org Recipe JSON-LD from accessible HTML web links or saved HTML files
- Import local plain-text and Recipe JSON-LD files; attach screenshot/photo or PDF originals
- Keep original sources offline alongside recipes, when the original was successfully captured
- Export/restore recipes, collections, photos and offline originals in a JSON backup
- Upgrades existing IndexedDB `recipe-pocket` v1 database to v2 without discarding recipes

## Important import limits
This is an offline-first web app, not a native SwiftUI app. Many websites disallow cross-origin browser requests, so pasting a link may not extract their recipe. Use an exported HTML file or paste recipe text in that case. PDF and photo imports retain the originals for offline use, but automatic OCR and PDF text extraction are **not** reliably available in iPhone Safari. The import review screen therefore asks for manual transcription/pasting instead of inventing ingredient amounts. Recipe photos from remote websites are only saved offline when their image server permits browser fetching; otherwise attach a photo manually.

## Deploy
Upload `index.html`, `app.js`, `styles.css`, `sw.js`, `manifest.webmanifest`, `icon.svg`, and `.nojekyll` to the **root** of your GitHub Pages repository. Select GitHub Pages → Deploy from `main` / root. Your installation should update automatically. If old version stays visible, fully close/reopen the Home Screen app or refresh in Safari.

## Privacy and backup
Recipes stay in IndexedDB on this device, not GitHub. Keep periodic backups in Files. Browser data clearing or app removal may delete local data. No sync across devices included.

## Updating an existing GitHub Pages install
Keep the repo name, GitHub Pages address, and IndexedDB database `recipe-pocket` unchanged to retain existing local recipes. Export a full backup before uploading. Backups from `Recipe Pocket` and `Dishkeep` are both accepted. This is a working name; competing products already use Dishkeep, so trademark clearance is needed before any public App Store launch.
