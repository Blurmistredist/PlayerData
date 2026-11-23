REAWAKENING PLAYER DATA — FEATURE UPDATE

CONTENTS
- index.html: website, particle/background/music controls, highlight display and editors
- players-data.json: public player/contributor/badge/cape data
- manus-storage/: existing website images and assets

NEW FEATURES
- Badge Legend is collapsible.
- Online accepted players are sorted by awarded badge count (highest first); offline players remain below all online players. Existing online/offline filters still apply. All players remain in the same grid.
- Ambient floating pixel particles with controls for count, speed, spread, glow colour, pixel colour and variable size.
- Background base colour, ambient glow colour and glow intensity controls.
- Music controls in the header: play/pause and next track. Add audio files to manus-storage/Playlist/ and enter their paths in Music & Playlist Editor. Browsers may block autoplay until the visitor interacts; the play button is always available.
- Highlights section appears at the bottom only when at least one highlight is saved. Upload images to manus-storage/highlight-image/ and enter the path in Highlight Editor. The JSON stores only title, description and image path; image files remain in GitHub.
- New settings are saved in the website data JSON and should be exported after editing.

PUBLISHING
1. Extract the ZIP and upload/replace the repository contents, keeping manus-storage/ paths intact.
2. In editor mode, make changes and export players-data.json.
3. Replace the repository's players-data.json with the exported file and commit/push.
4. Upload any new images/audio files into their specified manus-storage/ folders and commit/push those files too.

NOTES
This is a static GitHub Pages site. Audio autoplay depends on browser permission/user interaction. The owner password is client-side and is only a convenience lock, not secure authentication.
