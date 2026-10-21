# Weekly Laser Cutting Report — iPhone-ready web app

## Features
- Add one laser production job per entry
- Date and automatically filled day
- Sales Order No., Product Type / Model, Time Taken (minutes), Sheets Used, Description
- Edit/delete records
- Automatic weekly totals
- Choose week start/end and export only those jobs to Excel
- Share Excel using the iPhone share sheet when supported
- Saves data in this browser on this device
- PWA manifest/service worker included

## Publish it so it can be added to the iPhone Home Screen
This app must be hosted on an HTTPS website before iOS can install it as a Home Screen web app. This ZIP is not a public URL by itself.

One straightforward path:
1. Create/sign in to a GitHub account.
2. Create a new repository, for example `weekly-laser-report`.
3. Upload `index.html`, `manifest.webmanifest`, and `sw.js` to the repository root.
4. In repository Settings → Pages, enable deployment from the `main` branch and root folder.
5. Wait for GitHub Pages to provide the public HTTPS URL.
6. Open that URL in Safari on the iPhone → Share button → Add to Home Screen → Add.

## Data / privacy limitation
Records are stored in browser local storage on that device only. They do not automatically sync between devices. Export the Excel report weekly as a backup. Do not clear Safari website data unless you have backed up the report.

## Excel export
The app uses the SheetJS library from a CDN, so Excel export/share requires internet access.
