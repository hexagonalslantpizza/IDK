# IDK — Sandbox PVP

A browser-based 3D low-poly sandbox/PVP prototype.

## Demo 004

Current features:
- First-person movement and mouse look
- Low-poly outdoor test map
- Nine-slot hotbar
- Arcade pistol and reload
- Build menu and crate placement
- Dynamic crates with basic gravity and collision
- Grab tool to pick up and drop crates
- Weld tool to connect crates
- Thrusters that push equipped crates
- Fictional arcade bomb with countdown and crate knockback
- Vehicle seat, engine, four wheels, and wire tool
- Vehicles require an engine connected to at least two wheels before they can be driven
- Press F while aiming at a seat to sit; WASD drives; press F again to exit
- Trees can be knocked down by a fast welded assembly of at least two crates; a single crate cannot knock them down

## Controls

- WASD: walk or drive while seated
- Mouse: look
- Space: jump
- Shift: sprint
- 1: pistol
- 2: grab/drop crate
- 3: weld two crates
- 4: attach thruster; hold E while aiming at a thruster-equipped crate to fire it
- 5: place arcade bomb
- 6: attach a seat to an aimed-at crate
- 7: attach an engine to an aimed-at crate
- 8: attach up to four wheels to an aimed-at crate
- 9: wire tool: click the engine, then click each wheel to connect it
- F: sit in an aimed-at seat or exit the current seat
- Q: drop a held crate
- R: reload
- B: open/close build menu
- Right click: remove an aimed-at crate
- Esc: release mouse

## Run locally

Open `index.html` through a local web server (ES modules are not supported reliably from a `file://` URL). For example:

```bash
py -m http.server 8000
```

Then visit http://localhost:8000.

Three.js is stored in `vendor/three.module.js` and loads locally.

## Development status

This is a local single-player development build. Multiplayer networking and synchronized physics are not implemented. The latest vehicle and tree mechanics have not been browser-tested yet.
