# robosimu

https://robosimu.github.io

---

**Forward Kinematics** — A 3-DOF planar arm. Move joint angles with sliders, watch the end-effector follow. Every position on the canvas is computed from three numbers: θ1, θ2, θ3. The trace shows where the TCP has been.

**Inverse Kinematics** — The reverse problem: click anywhere in the workspace, the arm solves for the joint angles that get the gripper there. Reveals why IK is harder than FK — there are often multiple solutions, and some targets are unreachable.

**Differential Drive** — A two-wheeled robot navigating a space. Left and right wheel speeds determine both velocity and turning rate. PID controller keeps it on a path despite accumulated odometry error.

**SLAM** — The robot doesn't know the map. It builds one while moving, reconciling sensor readings against what it's already seen. Watch uncertainty grow and collapse as landmarks are re-observed.

**Mobile Manipulation** — A mobile base with an arm. The base navigates to a position; the arm reaches for an object. Coordination between whole-body motion and end-effector precision.
