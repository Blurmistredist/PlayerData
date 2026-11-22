HOMELIFE PLAYERS — GITHUB PAGES PACKAGE

CONTENTS
- index.html: standalone Players tab recreation
- players-data.json: public player/team/badge/cape data from the supplied backup
- manus-storage/: profile pictures, badge art, cape art, skins and other referenced images

PUBLISH TO GITHUB PAGES
1. Extract this ZIP.
2. Open your GitHub repository (or create a new one).
3. Upload the CONTENTS of this folder to the repository root. Keep index.html, players-data.json and manus-storage together.
4. In GitHub, open Settings > Pages.
5. Choose Deploy from a branch, select your branch (usually main) and folder / (root), then Save.
6. Open the Pages URL after deployment finishes.

PLAYERS & BADGES SETTINGS SETUP
1. Upload the files to GitHub Pages and open your published Players page.
2. Click Players & Badges Settings.
3. On the first visit in that browser, it will ask you to create a password and confirm it.
4. After setup, click Players & Badges Settings and enter that password whenever you want to unlock the editor.
5. The password is stored in that browser's local storage. If you clear site data or switch browsers/devices, you will need to set it up again.

IMPORTANT SECURITY / PUBLISHING LIMITS
This is a static GitHub Pages site. The password is stored in local storage and the check runs in client-side JavaScript. This is only a convenience lock and cannot securely restrict access to a determined visitor. Do not put secrets or private information in the static site. For genuine owner-only authentication and shared edits that instantly update every visitor's view, the site needs a private server/API or another authenticated backend.

Edits made in Players & Badges Settings are saved in that browser's local storage. They do not automatically change the public JSON file for other visitors. Use Download player data to download homelife-players-data.json. To publish those changes, replace the repository's players-data.json with the downloaded file and commit/push it. Import data can restore a previously exported JSON file. Reset restores the original data shipped in this package.

SCOPE
The package recreates the Players directory, Realm Team cards, accepted-player search, player profile views, badge legend/search/category filters, cape and badge collections, social links, skin image display, and a Players & Badges management dashboard based on the supplied Owners Dashboard screenshots. The dashboard includes accepted-player profile controls (including awarded badge and cape assignment), Realm Team profile controls, cape collectible creation/editing/deletion, local export/import, and reset. The dashboard waits for players-data.json to finish loading before allowing the editor to open. Normal Badge settings and Event Badge settings are intentionally excluded, as are Premium Account, Website Activity, Application Search, and unrelated dashboard settings. The source's live server functions are not available on GitHub Pages; presence and directory data are a snapshot until manually updated.

DATA HANDLING
Only public player-directory fields needed for the Players experience were included. Account password hashes, claim/session credentials, application search records, and website activity records were not copied into the site package.
