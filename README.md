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

Three.js is stored in `vendor/three.module.js` and loads locally. After you download the project files, the game does not need an internet connection.

## Development status

This is a local development build for now. Do not treat it as a published web release.

## Planned next

Test movement, collision, crate placement, hotbar selection, reload, and jump settings. Add further building and PVP systems only after the current demo is tested. Multiplayer will be designed as a separate client/server layer later; this demo is single-player only.
