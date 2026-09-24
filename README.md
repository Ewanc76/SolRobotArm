# SolRobotArm

An open, experimental robot-arm project growing out of a working LEGO Technic prototype.

The prototype proved that a compact four-motor arm can lift useful objects while keeping most motor mass toward the rear for counterbalance. The next phase is a purpose-designed, 3D-printable arm with Arduino/ESP32 control.

## Current prototype

- LEGO Technic structure
- Four powered functions
- Three motors mounted toward the rear for counterbalance
- Power Functions servo near the final large joint
- Worm-drive elbow reduction
- One Powered Up hub can support the current four-motor layout
- Lifted a 100 g wrench from ground level to vertical
- Lifted a 28.15 g bottle with the arm extended
- Roughly 5–10 mm of end-effector play from worm-gear backlash
- A 100 g load at the claw approached the extended-arm limit

## Printed-arm direction

- NEMA 17 stepper for the shoulder
- NEMA 14 stepper for the elbow
- Smaller geared steppers with ULN2003 drivers for experiments or light-duty axes
- Arduino Uno R3 and ESP32-WROOM available for control development
- Modular joints so motors and transmissions can be changed without redesigning the whole arm

Motor sizes, reductions, bearings, and power requirements remain subject to bench testing.

## Project goals

1. Document and characterize the LEGO prototype.
2. Build a single-joint test stand.
3. Measure torque, speed, backlash, repeatability, current, and temperature.
4. Develop modular printable shoulder and elbow joints.
5. Add safe manual control, homing, and travel limits.
6. Grow toward recorded motion and simple autonomous tasks.

## Repository map

- [Hardware inventory](docs/hardware-inventory.md)
- [Mechanical prototype](docs/mechanical-prototype.md)
- [Design decisions](docs/design-decisions.md)
- [Roadmap](docs/roadmap.md)
- [Project log](docs/project-log.md)
- [Firmware workspace](firmware/README.md)
- [CAD workspace](cad/README.md)
- [Media guide](media/README.md)

## Status

Early prototype and architecture phase. Expect experiments, redesigns, ugly brackets, surprisingly capable LEGO, and measurements that invalidate our favorite ideas.
