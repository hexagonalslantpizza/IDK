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

Improve collision and building placement, then add interactive objects and the first PVP systems. Multiplayer will be designed as a separate client/server layer later; this demo is single-player only.
