# Robosimu

**Robotics control problems**, visualized in the browser. Each demo isolates one concept — no physics engine, no setup, just the math made interactive.

Live at [robosimu.github.io](https://robosimu.github.io)

## The core idea

A robot arm doesn't "know" where its hand is — it only knows its joint angles. Every control problem in robotics comes down to the relationship between **joint space** (angles) and **Cartesian space** (positions in the world).

- **Forward kinematics** — given joint angles, where is the end-effector?
- **Inverse kinematics** — given a target position, what angles produce it?
- **Path planning** — how do you move from A to B without hitting anything?
- **SLAM** — how do you navigate when you don't have a map?

These problems look simple. They're not. Each demo shows exactly where and why they get hard.

## Demos

| # | Demo | Concept |
|---|------|---------|
| 01 | [Forward Kinematics](https://robosimu.github.io/01-fk/) | Three joint angles fully determine end-effector position. Move sliders, watch the TCP trace. |
| 02 | Inverse Kinematics | The reverse: click a target, the arm solves for joint angles. Multiple solutions exist; some targets don't. |
| 03 | Differential Drive | Wheel speeds determine velocity and turn rate. PID keeps the robot on path despite odometry drift. |
| 04 | SLAM | The robot builds a map while moving. Watch uncertainty grow and collapse as landmarks are re-observed. |
| 05 | Mobile Manipulation | Base navigates; arm reaches. Whole-body coordination between locomotion and end-effector precision. |

01 is live. 02–05 are in progress.

---

Plain HTML/CSS/JS, no build step. `npx serve .` to run locally.
