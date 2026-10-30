SUJAN FIT OS — FREE OFFLINE EDITION
===================================

START ON A WINDOWS/MAC PC
  1. Unzip this folder.
  2. Double-click index.html in Chrome, Edge, Safari or Firefox.
  3. Start using the dashboard, food diary, workout and sport logging.
  4. Your entries are saved privately in this browser on this device.

PHONE SETUP / INSTALLABLE APP
  For simple opening, move index.html to your phone and open it in a browser. Some mobile browsers restrict storage and installation when opening file:// files. For a more reliable installable app, use a FREE static host (e.g. GitHub Pages) to host this entire folder over HTTPS. You do NOT need a paid service, account with a database, or API key. Once the page is loaded/installed over HTTPS, the service worker caches it for offline use.
  iPhone: open your hosted URL in Safari, use Share > Add to Home Screen.
  Android: open hosted URL in Chrome, browser menu > Install app / Add to Home Screen.
  You can also use any local HTTP server on your computer (e.g. python -m http.server 8000) for local testing; a localhost/HTTPS origin is required for service worker support.

IMPORTANT DATA LIMITATIONS
  - The application does NOT automatically sync a phone with a PC. Each browser/device has its own local database.
  - To move/backup records: Settings > Download complete backup, then Settings > Restore / replace or Import / merge on the other device.
  - Clearing site data, private browsing, changing to a different hostname, reinstalling certain browsers or device failure can erase local storage. Export JSON backups often.
  - This is offline software without registration, passwords, accounts, external trackers, or hosted database fees. Anyone who can access your unlocked device/browser may access the entries.
  - Cloud AI, barcode scanning, wearable sync, background push notifications and verified food APIs are NOT provided.
  - The coach uses rules and the meal plan uses editable sample templates. Nutrition values and grocery costs are estimates, not verified product labels. Check allergens and medical needs yourself.
  - This is not professional medical or dietetic advice.
  - Body photos are compressed and saved with the database, so exports can become large.

FILES
  index.html             Fully functional interface, CSS and JavaScript, self-contained.
  sw.js                  Offline PWA cache when served over HTTPS / localhost.
  manifest.webmanifest   Installable PWA metadata.
  icon.svg               App icon.

PRIVACY
  Zero third-party scripts. No data sent to external services by the app.
  No paid API keys, subscriptions or recurring charges.

MORE
  This is an independent offline product, NOT the Supabase/Next.js online starter project. Use only one version as your primary data store. Backup exports are from this offline version.

FREE PUBLIC URL WITH OFFLINE INSTALLATION (OPTIONAL)
  1. Create a free GitHub account, create a public repository named sujan-fit-os.
  2. Upload index.html, sw.js, icon.svg and manifest.webmanifest to the repository root.
  3. In repository Settings > Pages, set Source to Deploy from a branch, choose main / root.
  4. Open the URL GitHub Pages provides and Add to Home Screen (iPhone or Android).
  5. Load the site once while online to cache the PWA. It works offline afterwards.
  6. Your fitness records are still stored only on the current device, NOT on GitHub.
  7. Every device/browser keeps separate records. Transfer using JSON backup/import.
  Free GitHub Pages availability and limits are governed by GitHub's current terms.

CHECK THE APP
  From this folder, run: node tests/basic.test.cjs
  No node packages need to be installed. Node 18 or newer is recommended.
  Browser verification on your specific device/browser is still advisable.
