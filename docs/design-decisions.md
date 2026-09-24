# Design decisions

This file records current choices and the reasoning behind them. Decisions can change when test data disagrees.

## DD-001 — Prove mechanisms before printing a whole arm

**Status:** Accepted

Build a single-joint test stand first. It is faster and cheaper to discover insufficient torque, poor bearings, excessive backlash, or overheating on one module.

## DD-002 — Use modular joints

**Status:** Accepted

Motor mounts, reductions, arm links, and electronics should be separable. A motor or transmission change should not require rebuilding the entire arm.

## DD-003 — NEMA 17 shoulder and NEMA 14 elbow

**Status:** Current direction; requires measurement

These motors offer a more credible starting point for the primary joints than hobby servos or very small geared steppers. Final selection depends on measured torque after reduction, total moving mass, power, heat, speed, and holding behavior.

## DD-004 — Keep small geared steppers in the experiment pool

**Status:** Accepted

A 28BYJ-48-style stepper and ULN2003 board remain useful for inexpensive control experiments, light-duty axes, indicators, or test fixtures even if they are unsuitable for the shoulder and elbow.

## DD-005 — Favor rear-mounted mass

**Status:** Accepted

The LEGO prototype demonstrated that mounting three motors toward the rear materially improves balance. The printed design should preserve that advantage where practical through motor placement, remote drives, springs, or counterweights.

## DD-006 — Four powered functions for the first complete arm

**Status:** Provisional

Four functions produced a useful prototype without immediately creating a wiring and control swamp. Additional axes should justify their mass and complexity.
