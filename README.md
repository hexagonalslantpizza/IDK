# IDK — Sandbox PVP

A browser-based 3D low-poly sandbox/PVP prototype.

## Demo 002

Current features:
- First-person mouse-look
- WASD movement, sprinting, jumping, gravity
- Low-poly outdoor test map
- Nine-slot hotbar (pistol in slot 1)
- Arcade-style pistol with a 12-shot magazine, reserve ammo, reload, and 0.3-second firing cooldown
- Visual shot effect (no enemy damage system yet)
- Build menu with wooden crate placement
- Crates are placed at the point under the crosshair
- Adjustable jump setting in the build menu
- Remove a crate by aiming at it and right-clicking

## Controls

- WASD: move
- Mouse: look
- Space: jump
- Shift: sprint
- 1–9: select hotbar slot
- Left click: fire pistol, or place a crate in build mode
- R: reload
- B: open/close build menu
- Right click: remove an aimed-at crate
- Esc: release mouse

## Run locally

Open `index.html` through a local web server (ES modules are not supported reliably from a `file://` URL). For example, with Python installed:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

Three.js currently loads from jsDelivr, so this development version requires an internet connection.

## itch.io HTML5 compatibility

The project is being developed for itch.io's **HTML5** game format.

Before the first itch.io upload, the release package should:
- Be a ZIP archive with `index.html` at the ZIP's top level.
- Include every required JavaScript file, model, texture, and sound.
- Include a local copy of the Three.js dependency instead of relying on the development CDN.
- Be tested at the embedded game sizes used by itch.io.

Do not upload the GitHub repository ZIP as a finished release yet: the dependency is still loaded from an external CDN, and the release package has not been assembled or tested on itch.io.

## GitHub Pages

In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select **main** and **/(root)**, then save. The site will be published at the repository's GitHub Pages address once deployment finishes.

## Planned next

Test movement, collision, crate placement, hotbar selection, reload, and jump settings. Add further building and PVP systems only after the current demo is tested. Multiplayer will be designed as a separate client/server layer later; this demo is single-player only.
