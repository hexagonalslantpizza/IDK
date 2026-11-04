# IDK — Sandbox PVP

A browser-based 3D low-poly sandbox/PVP prototype.

## Demo 005

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
- Circuit parts: toggle switches, proximity sensors, motors, and gears
- Logic wiring: connect a switch or sensor to a motor; connect a motor to a gear
- Simple beams, hinged connections, and ropes between crate frames
- Glass panels that shatter on strong impacts or nearby blasts; wooden beams splinter
- Fire spreads between nearby wooden crates and trees; burning objects turn black after 20 seconds and are removed after another 10 seconds
- Fire extinguisher tool sprays toward the crosshair and puts out nearby flames
- Welds, ropes, and hinges can break under strong stress or explosions
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
- 9: wire tool: connect engine to wheels, switches/sensors to motors, or motors to gears
- 0: select a switch and click it to toggle on/off
- Mouse wheel: cycle through all 18 tools
- 11: sensor; attach to a crate to detect nearby crates
- 12: motor; connect a switch or sensor to activate it
- 13: gear; connect it to a motor to make it rotate
- 14: wooden beam; attach it to a crate frame
- 15: hinge; click two crate frames to connect them
- 16: rope; click two crate frames to connect them
- 17: glass panel; attach it to a crate frame
- 18: fire extinguisher; hold left click while aiming toward a fire
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

This is a local single-player development build. Multiplayer networking and synchronized physics are not implemented. The latest engineering, destruction, fire, and vehicle systems have not been browser-tested yet. These are simplified prototype physics, not full rigid-body simulation.
