# 2D Bouncing Ball Simulation (OpenGL Physics)

# Overview

This project is a 2D physics-based simulation of a bouncing rubber ball developed using C++ and OpenGL (GLUT). The ball follows realistic motion under gravity and gradually loses height after each bounce until it comes to rest.

The simulation is implemented using kinematic equations for horizontal and vertical motion, ensuring physically accurate behavior.

---

# Objectives

* Simulate realistic bouncing motion using physics equations
* Apply kinematic formulas for projectile motion
* Implement energy loss after each collision with the ground
* Visualize motion using OpenGL animation techniques

---

# Features

*  Realistic bouncing ball motion
*  Gradual energy loss after each bounce
*  Smooth animation using GLUT timer
*  Physics-based position updates (no shortcuts)
*  Optional keyboard control for speed

---

# Physics Model

The ball motion is calculated using standard kinematic equations:

### Horizontal Motion:

x = vₓ × t

### Vertical Motion:

y = vᵧ × t − (1/2) g t²

Where:

* vₓ = horizontal velocity
* vᵧ = initial vertical velocity
* g = gravitational acceleration

---

# Bouncing Logic

When the ball hits the ground:

* Vertical velocity is reversed:

  vᵧ = −e × vᵧ

* `e` is the coefficient of restitution (energy loss factor)

Each bounce reduces the height until:

vᵧ ≈ 0 → ball stops

---

# Controls
| Key | Function |
|-----|----------|
| `→` | Increase horizontal velocity |
| `←` | Decrease horizontal velocity |
| `↑` | Increase vertical velocity |
| `↓` | Decrease vertical velocity |
| `PgUp` | Increase gravitational acceleration |
| `PgDn` | Decrease gravitational acceleration |
| `Space` | Pause/Play simulation |
| `R` | Reset simulation |
| `ESC` | Exit program |

---

# Technologies Used

* C++
* OpenGL
* GLUT / FreeGLUT
* Classical Mechanics (Kinematics)

---

---

# Preview

<img width="624" height="629" alt="Screenshot 2026-04-25 124432" src="https://github.com/user-attachments/assets/a10c63b7-012b-4a00-8318-9f08911f00bc" />


---

# Learning Outcomes

* Applying physics equations in simulations
* Understanding motion under gravity
* Implementing collision and energy loss
* Using GLUT timers for real-time animation

---

# Notes

* The simulation assumes a flat ground surface
* Air resistance is ignored
* Energy loss is controlled manually using a damping factor

---

# Author
Maya Ramy Essam
Biomedical Engineering Student
Cairo University

Interested in Simulation, Physics-Based Systems, and Computer Graphics

