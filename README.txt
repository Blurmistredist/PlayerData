REAWAKENING PLAYER DATA

This is a static GitHub Pages website. Upload the contents of this folder to the same repository location as your existing site files.

FEATURES IN THIS BUILD
- Smp Contributor profiles use a Discord-inspired banner layout with the avatar overlapping the lower-left edge of the banner and a separate nameplate below it.
- Contributor profile tabs contain STATUS, the selected status value (Ongoing or Stopped associating since YYYY-MM-DD), About, Badges, and Social links.
- Optional contributor status words are displayed separately under STATUS WORDS.
- Contributor name, nameplate, and profile-tab colours each support solid colour or a two-colour gradient, with a direction selector and live preview in the editor.
- Contributor banner paths use manus-storage/distributor-banner/.
- Ordinary player cards stay in one directory grid. In All view, online/playing/away players sort above offline players. Search filters include All, Online only, and Offline only.
- Offline ordinary player cards retain their faded/darker appearance.

PLAYER DATA PUBLISHING
1. Unlock Players & Badges Settings.
2. Make your edits.
3. Export/download the player JSON from the editor.
4. Replace players-data.json in this GitHub repository with the exported JSON file.
5. Commit and push. Visitors will load the published JSON.

The editor's working data is browser-local until exported and uploaded. The shared password in index.html is a convenience lock only; static GitHub Pages cannot provide secure authentication.

ASSETS
Keep the manus-storage folder alongside index.html and players-data.json. Use exact relative paths, for example:
manus-storage/distributor-banner/example.png
manus-storage/capes-textures/example.png
manus-storage/title/season3.png
