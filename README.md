# IDK — Sandbox PVP

A browser-based 3D low-poly sandbox/PVP prototype.

## Demo 001

Current features:
- First-person mouse-look
- WASD movement, sprinting, jumping, gravity
- Low-poly outdoor test map
- Free placement of wooden crates
- Remove a crate by aiming at it and right-clicking

## Run locally

Open `index.html` through a local web server (ES modules are not supported reliably from a `file://` URL). For example, with Python installed:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

Three.js is loaded from jsDelivr, so an internet connection is required.

## GitHub Pages

In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select **main** and **/(root)**, then save. The site will be published at the repository's GitHub Pages address once deployment finishes.

## Planned next

Improve collision and building placement, then add interactive objects and the first PVP systems. Multiplayer will be designed as a separate client/server layer later; this demo is single-player only.
