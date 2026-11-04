# IDK — Sandbox PVP

A browser-based 3D low-poly sandbox/PVP prototype.

## Demo 003

Current features:
- First-person mouse-look
- WASD movement, sprinting, jumping, gravity
- Low-poly outdoor test map
- Nine-slot hotbar
- Arcade-style pistol with a 12-shot magazine, reserve ammo, reload, and 0.3-second firing cooldown
- Build menu with wooden crate placement at the crosshair
- Adjustable jump setting
- Dynamic, unanchored crates with basic gravity and collision
- Grab tool to pick up, move, and drop crates
- Weld tool to connect two crates so they move together
- Thruster tool that attaches to a crate and pushes it while activated
- Fictional arcade bomb with a short countdown and crate-only knockback
- Right-click to remove an aimed-at crate

## Controls

- WASD: move
- Mouse: look
- Space: jump
- Shift: sprint
- 1: pistol
- 2: grab/drop crate (left click or Q to drop)
- 3: weld two crates (click the first, then the second)
- 4: attach a thruster; aim at a thruster-equipped crate and hold E to fire it
- 5: place an arcade bomb (3-second countdown; launches nearby crates)
- R: reload
- B: open/close build menu
- Right click: remove an aimed-at crate
- Esc: release mouse

## Run locally

Open `index.html` through a local web server (ES modules are not supported reliably from a `file://` URL). For example, with Python installed:

```bash
py -m http.server 8000
```

Then visit http://localhost:8000.

Three.js is stored in `vendor/three.module.js` and loads locally. After you download the project files, the game does not need an internet connection.

## Development status

This is a local development build for now. It has not been browser-tested after the latest tool changes. The current build is single-player only; multiplayer networking and synchronized physics are not implemented yet.
