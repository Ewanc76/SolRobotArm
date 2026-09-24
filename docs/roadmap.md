# Roadmap

This roadmap is intentionally experimental. Results outrank the order written here.

## Phase 0 — Capture the working prototype

- [ ] Photograph all sides of the LEGO arm
- [ ] Record arm-segment lengths and joint ranges
- [ ] Map every motor to its function and port
- [ ] Record gearing at each joint
- [ ] Repeat the 28.15 g and 100 g tests with consistent poses
- [ ] Add the cleaned Rebrickable inventory exports

## Phase 1 — Single-joint test stand

- [ ] Select the initial NEMA motor and driver
- [ ] Design a printable motor mount and output bearing
- [ ] Add a known-length lever arm
- [ ] Measure lifting torque across speeds
- [ ] Measure holding current and temperature
- [ ] Quantify backlash and repeatability
- [ ] Add a homing switch

## Phase 2 — Electronics foundation

- [ ] Establish a power budget
- [ ] Choose Arduino Uno, ESP32, or a split-controller architecture
- [ ] Implement non-blocking motor control
- [ ] Add emergency-stop behavior
- [ ] Add soft travel limits
- [ ] Store calibration values
- [ ] Document connectors and wire colors

## Phase 3 — Shoulder and elbow

- [ ] Convert the best test-joint design into modular joints
- [ ] Add bearings and intentional structural load paths
- [ ] Test unloaded synchronization
- [ ] Test payloads at defined reach
- [ ] Compare counterweight, spring, and motor-placement strategies

## Phase 4 — Wrist and end effector

- [ ] Define a standard tool interface
- [ ] Prototype a lightweight gripper
- [ ] Add grip-force or current limiting
- [ ] Test objects with varied shapes and compliance

## Phase 5 — Control

- [ ] Manual jog controls
- [ ] Recorded pose playback
- [ ] Coordinated multi-axis movement
- [ ] Simple inverse-kinematics experiment
- [ ] Wireless interface if the ESP32 is selected

## Someday / strange ideas worth keeping

- Tool-changing wrist
- Camera-guided object pickup
- LEGO and printed-arm comparison rig
- Teleoperation from a custom controller
- A machine tending a tiny imaginary factory
