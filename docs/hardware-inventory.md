# Hardware inventory

This is the known starting inventory. Quantities and exact variants should be verified at the bench before wiring or CAD is finalized.

## Controllers

| Item | Quantity | Notes |
|---|---:|---|
| Arduino Uno R3 | 1 | Good for simple motor and sensor experiments |
| ESP32-WROOM | 1 | Candidate for wireless control and higher-level coordination |
| LEGO Powered Up hub | 1+ | The current four-motor prototype can operate from one hub |

## Motors and actuators

| Item | Quantity | Notes |
|---|---:|---|
| LEGO Power Functions Large motor | 4 | Available for prototype joints |
| LEGO Power Functions Medium motor | 3 | Available for lighter functions |
| LEGO Power Functions Servo | 1 | Used near the final large joint in the prototype |
| LEGO Powered Up Large motor | 2 | Position-aware control is worth investigating |
| NEMA 17 stepper | Planned | Current shoulder design direction |
| NEMA 14 stepper | Planned | Current elbow design direction |
| 28BYJ-48-style geared stepper | Candidate | Useful for test rigs or lighter axes |
| ULN2003 driver board | Candidate | Typical driver for 28BYJ-48-style steppers |

## Power and motor control

| Item | Quantity | Notes |
|---|---:|---|
| 7.4 V Li-ion RC battery | 1+ | Verify capacity, connector, and discharge rating |
| UBEC | Planned | Use a regulated supply appropriate to logic and servos |
| Traxxas Slash brushed ESC | 1 | Available; probably not required for the stepper architecture |
| Hobbywing brushless ESC | 1 | Available; probably not required for the initial arm |
| Generic multi-channel battery boxes | 2 | Ten total channels available |
| Modified Powered Up hub | 1 | Fitted with LiPo connector; previously used around 6–7.4 V |

## Before connecting power

- Confirm each motor's rated voltage and stall current.
- Never drive a motor directly from an Arduino or ESP32 GPIO pin.
- Establish a common ground where the chosen driver topology requires it.
- Add current limiting, fusing, or another deliberate fault-protection strategy.
- Test one unloaded axis before assembling the full arm.
- Document battery polarity and connector modifications.

## Measurements still needed

- Joint torque at representative speeds
- Current draw while idle, moving, holding, and stalled
- Stepper temperature during sustained holding
- Backlash at each transmission stage
- Actual arm-segment dimensions and masses
- Repeatability after approaching a target from both directions
