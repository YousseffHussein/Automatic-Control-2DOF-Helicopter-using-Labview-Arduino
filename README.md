# 🚁 2-DOF Helicopter Control Project

This project explores the design and implementation of a control system for a **2-degree-of-freedom (2-DOF) helicopter beam**. It was developed as part of the Automatic Control 2 course.

## 📄 Description

The goal of this project was to regulate the dynamics of a 2-DOF helicopter beam, achieving stable and precise pitch and yaw control.

- A **PID controller** was implemented to minimize oscillations, reduce steady-state error, and improve system stability.
- A **PD controller** was initially tested but proved inadequate due to high steady-state error. Introducing the integral component (I) in the PID controller significantly improved performance.

## 🛠️ Hardware Components

- Arduino Uno
- Motor Driver L298 (replacing DRV8871 after failure)
- 720 Coreless Motors with 75mm Propellers
- Rolling Bearings (3 pieces)
- 3D-Printed Shafts (for vertical height and swinging motion)
- Acrylic Beam and Base
- Wooden Base Block
- Accelerometer/Gyroscope
- Batteries

These components were assembled into a mechanical system capable of simulating pitch and yaw motions.

## 🧮 System Modeling & Control

- A **state-space model** was derived using the Euler-Lagrange method and linearized under small-angle assumptions.
- Inputs: Voltages to main and tail rotors
- Outputs: Pitch angle (θ) and yaw angle (φ)
- Due to the coupling between pitch and yaw channels, the system was treated as multivariable.

## 🖥️ Software & Simulation

- **LabVIEW** was used to implement and simulate the control algorithms.
- The **LINX toolkit** enabled serial communication between LabVIEW and Arduino.
- Challenges encountered:
  - Serial port conflicts
  - Difficulty calibrating the accelerometer and gyroscope readings

Simulations confirmed the effectiveness of PID control for stabilizing both pitch and yaw.

## ✅ Results & Conclusion

- The PID controller provided stable, precise control compared to the initial PD-only design.
- Future work may explore:
  - Advanced control methods (e.g., adaptive PID, Model Predictive Control)
  - Experimental validation on a physical helicopter model

---

Project Demo:




https://github.com/user-attachments/assets/710abbce-eb3b-43fb-80ba-54153292b041











