# Mechanical prototype

## What worked

The LEGO Technic prototype established several useful design principles:

- Geared-down shoulder motion can handle useful loads.
- Replacing the elbow's short-travel linear actuator arrangement with continuous gearing greatly increased usable motion.
- Rear-mounted motors materially improve balance.
- Keeping a motor close to the joint it serves reduces distal structural load.
- Four powered functions are enough for a useful first arm.
- One Powered Up hub can support the current motor count.

## Recorded load tests

| Test object | Mass | Configuration | Result |
|---|---:|---|---|
| Wrench | 100 g | Moved from ground level to vertical | Successful without obvious failure |
| Bottle | 28.15 g | Arm extended | Successful |
| Test load | 100 g | At claw near maximum extension | Mechanism approached its limit |

These are practical observations, not formal payload ratings. A repeatable fixture and defined poses are needed before publishing specifications.

## Known limitation: backlash

The worm-gear elbow exhibits roughly 5–10 mm of observed play at the working end. Possible sources include:

- Worm-to-gear clearance
- Axle and bearing clearance
- LEGO pin and beam compliance
- Accumulated play across multiple joints
- Structural twist under load

Potential experiments:

1. Measure backlash at the joint and end effector separately.
2. Approach identical positions from both directions.
3. Add preload or opposing gears.
4. Compare planetary, belt, cable, and printed gear reductions.
5. Determine whether software compensation is adequate for the intended tasks.

## Printed-arm architecture

The printed version should be modular enough to swap motors and transmissions without redrawing the entire arm:

- Base
- Shoulder module
- Upper arm
- Elbow module
- Forearm
- Wrist interface
- End-effector interface
- Electronics enclosure

The first printed mechanism should be a single-joint bench module, not a whole arm. That lets us characterize torque, backlash, speed, heat, and repeatability before multiplying one bad idea across several axes.
