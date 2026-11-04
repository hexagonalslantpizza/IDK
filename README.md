# FREEFORM — Sandbox PVP

A browser-based 3D sandbox prototype.

## Current demo

- First-person movement, mouse look, sprinting, and adjustable jump height
- Four-slot hotbar: pistol, grab, weld, and fire extinguisher
- Construction menu for buildable objects
- Free placement on ground and world surfaces
- Crates stack, collide, and support the player
- Seats, engines, wheels, switches, sensors, motors, gears, beams, and glass place at the exact surface point under the crosshair, including on a crate
- Hinge and rope endpoints are anchored at the exact two points selected on separate crates
- Grab tool picks up crates and build parts; held objects can be rotated and tilted
- Thrusters, arcade bombs, simplified vehicles, circuit logic, destruction, and spreading fire

## Controls

- WASD: move or drive while seated
- Mouse: look
- Space: jump
- Shift: sprint
- 1–4: pistol, grab, weld, extinguisher
- Mouse wheel: cycle through hotbar tools
- B: open/close build menu
- Choose a build item, press DONE, then click the exact spot in the world where it should be placed
- Z / X: rotate a held object left/right
- C / V: tilt a held object while holding it
- Q: drop a held object
- F: sit in an aimed-at seat or exit
- R: reload pistol
- E: fire an aimed-at thruster-equipped crate
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

This is a local single-player development build. Multiplayer networking and synchronized physics are not implemented. The physics and engineering systems are simplified prototypes. JavaScript syntax has been checked, but the latest changes have not been browser-tested yet.
