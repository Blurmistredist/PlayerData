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

OWNER MODE SETUP
1. Open index.html in a text editor before uploading.
2. Find: const OWNER_PASSWORD = "CHANGE-THIS-OWNER-PASSWORD";
3. Replace the placeholder with a password of your choice.
4. Upload the changed index.html.
5. On the site, choose Owner Mode and enter that password.

IMPORTANT SECURITY / PUBLISHING LIMITS
This is a static GitHub Pages site. The owner password is embedded in downloadable client-side JavaScript, so it is only a convenience lock and cannot securely restrict access to a determined visitor. Do not put secrets or private information in it. For genuine owner-only authentication and shared edits that instantly update every visitor's view, the site needs a private server/API or another authenticated backend.

Edits made in Owner Mode are saved in that browser's local storage. They do not automatically change the public JSON file for other visitors. Use Export data to download homelife-players-data.json. To publish those changes, replace the repository's players-data.json with the downloaded file and commit/push it. Import data can restore a previously exported JSON file. Reset restores the original data shipped in this package.

SCOPE
The package recreates the Players directory, Realm Team cards, accepted-player search, player profile views, badge legend/search/category filters, cape and badge collections, social links, skin image display, and a local owner editor. Premium Account, Website Activity, and Application Search are intentionally omitted. The source's live server functions are not available on GitHub Pages; presence and directory data are a snapshot until manually updated.

DATA HANDLING
Only public player-directory fields needed for the Players experience were included. Account password hashes, claim/session credentials, application search records, and website activity records were not copied into the site package.
