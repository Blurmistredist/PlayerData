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
The package recreates the Players directory, Smp Contributor cards, accepted-player search, player profile views, badge legend/search/category filters, cape and badge collections, social links, interactive 3D skin/cape/Elytra viewer, and a Players & Badges management dashboard based on the supplied Owners Dashboard screenshots. The dashboard includes accepted-player profile controls (including awarded badge and cape assignment), Smp Contributor add/edit/delete controls, badge definition creation/editing/deletion, cape collectible creation/editing/deletion, Smp Contributor creation/editing/deletion, per-player default cape selection, Elytra visibility control in the 3D viewer, local export/import, and reset. The dashboard waits for players-data.json to finish loading before allowing the editor to open. Normal Badge settings and Event Badge settings are intentionally excluded, as are Premium Account, Website Activity, Application Search, and unrelated dashboard settings. The source's live server functions are not available on GitHub Pages; presence and directory data are a snapshot until manually updated.

DATA HANDLING
Only public player-directory fields needed for the Players experience were included. Account password hashes, claim/session credentials, application search records, and website activity records were not copied into the site package.

3D Minecraft skin viewer
- Player profiles use MinecraftCapes/minecraft-skin-viewer (https://github.com/MinecraftCapes/minecraft-skin-viewer), loaded as an ES module from esm.sh. It supports classic/slim skins and cape textures.
- The viewer supports drag rotation, auto-rotation, zoom, and an idle animation. It needs an internet connection to load the library and WebGL support in the browser.
- Profile image/skin/cape/badge paths are normalized to ./manus-storage/. Global cape texture paths are stored on each cape collectible and shared by all players. The title season choice is stored in siteSettings.titleSeason.
- Add the three title image files as manus-storage/title/season1.png, season2.png and season3.png. The selected title image is season3.png by default.
- Add the cape texture PNGs under manus-storage/capes-textures/ and set each global cape texture path in the editor.
- MinecraftCapes/minecraft-skin-viewer is MIT-licensed; see https://github.com/MinecraftCapes/minecraft-skin-viewer/blob/main/LICENSE.
- The previous package did not contain season1.png, season2.png, season3.png or the cape texture PNGs. Add those image files to the folders above for the title and cape previews to render.


Latest update:
- Added Change password control inside the unlocked Players & Badges Settings panel. It verifies the current password, then confirms a new password (minimum 6 characters). This browser-only password remains a convenience lock, not secure server authentication.
- Removed the large white Smp Contributor heading while keeping the small section label.
- Removed the 'Preview on skin' caption from cape tiles.
- Adjusted the MinecraftCapes viewer Elytra position closer to the player's back.
