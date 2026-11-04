# FREEFORM — Sandbox PVP

A browser-based 3D low-poly sandbox prototype.

## Current demo

- First-person movement, mouse look, sprinting, and adjustable jump height
- Low-poly outdoor test map
- Four-slot hotbar: pistol, grab, weld, and fire extinguisher
- Construction menu for buildable objects
- Free placement on surfaces, including the ground and the tops/sides of existing objects
- Crates can stack, collide, and support the player
- Player can jump and stand on crates and other world surfaces
- Grab tool can pick up crates and freely placed build objects; held objects are blocked by world geometry
- Weld tool connects crates
- Thrusters, arcade bombs, seats, engines, wheels, switches, sensors, motors, gears, beams, glass, hinges, and ropes
- Fire spreads between nearby wooden crates and trees; objects turn black after 20 seconds and disappear after another 10 seconds
- Fire extinguisher sprays toward the crosshair
- Simplified vehicle, circuit, destruction, and fire systems

## Controls

- WASD: move or drive while seated
- Mouse: look
- Space: jump
- Shift: sprint
- 1–4: select pistol, grab, weld, or extinguisher
- Mouse wheel: cycle through the four hotbar tools
- B: open/close the build menu
- In the build menu: choose an item, press DONE, then click in the world to place/use it
- F: sit in an aimed-at seat or exit
- Q: drop a held object
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

This is a local single-player development build. Multiplayer networking and synchronized physics are not implemented. The physics and engineering systems are simplified prototypes, not full rigid-body simulation. JavaScript syntax has been checked, but the latest changes have not been browser-tested yet.
