# Mech Forge VR: Credits

## 3D assets
- **RobotExpressive** (crew chief, hostile ground bots), by Tomás Laulhé ([Quaternius](https://quaternius.com)), modifications by Don McCurdy. License: **CC0 1.0** (public domain). Taken from the three.js examples (`examples/models/gltf/RobotExpressive`).

## Everything else
- The mech parts, hangar, terrain, survivors, drones, relays, buildings and particles are all generated in code (no external meshes).
- The textures (panels, hazard stripes, treads, concrete, grates) are drawn at runtime on canvases.
- The sounds (motors, servos, wind, jets, drill, cannon, explosions, alarms, UI) are synthesized at runtime with WebAudio. No sample files are used.

## Code and libraries
- [three.js](https://threejs.org) (MIT), including RoomEnvironment, UnrealBloomPass, SkeletonUtils, GLTFLoader and XRHandModelFactory.
- `src/robot-sim.js` is the robot physics module by Michael (team robotics expert). It covers traction, slope limits, battery thermal and capacity, motor heating, warnings and failures.
- The test emulator is [IWER](https://github.com/meta-quest/immersive-web-emulation-runtime) (MIT, Meta), used for development and testing only.
