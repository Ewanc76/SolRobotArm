# Firmware

Firmware will live here once the first motor-control experiment is defined.

## Likely progression

1. Command one unloaded motor.
2. Add acceleration and deceleration.
3. Add a homing switch.
4. Enforce hard and soft travel limits.
5. Store a calibrated zero position.
6. Coordinate two joints.
7. Add manual controls or a serial command protocol.

## Proposed layout

```text
firmware/
├── experiments/
│   └── single_joint/
├── lib/
│   ├── motion/
│   └── safety/
└── controller/
```

## Safety defaults

Firmware should fail stopped. On boot, disconnect, invalid command, limit violation, or watchdog timeout, motor commands should move to a defined safe state.

Do not place Wi-Fi passwords, access tokens, or other credentials in committed source files. Use a local untracked configuration file and provide a redacted example when networking is added.
