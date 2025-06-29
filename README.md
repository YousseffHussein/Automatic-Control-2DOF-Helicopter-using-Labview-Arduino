#  Automatic Control SISO System (.vi – LabVIEW Project)

## 📌 Project Description

This project demonstrates a **Single Input Single Output (SISO)** control system implemented using **LabVIEW**. The system simulates an automatic control loop where a **manual input signal** is tracked and matched by a **motor-driven output signal**, using real-time feedback and actuation logic.

The control logic is developed as a `.vi` file using **LabVIEW**, making use of analog signal acquisition, real-time comparison, and motor control based on error calculations.

---

## 🎯 Objectives

- Develop a closed-loop control system in **LabVIEW**.
- Use one potentiometer as **manual input** and another as a **feedback output**.
- Control a DC motor to align the output signal with the desired input.
- Demonstrate fundamental principles of **automatic control systems**, such as error correction, tolerance limits, and direction control.

---

## 🧰 Hardware Requirements

- ✅ NI DAQ or compatible analog/digital interface
- ✅ LabVIEW (with DAQmx drivers)
- ✅ Two potentiometers (manual and motor-attached)
- ✅ DC Motor
- ✅ Motor Driver (e.g., L298N)
- ✅ Power Supply
- ✅ USB cable (for communication/control)

---

## 🧠 How It Works

- **Input Potentiometer**: Sets the desired position or target value.
- **Output Potentiometer**: Connected to a DC motor, representing system output.
- **LabVIEW VI** reads both analog signals and continuously computes the **error**.
- If the error is greater than a defined **tolerance**, it sends control signals to rotate the motor in the required direction.
- Once the error is within the tolerance, the **motor stops**.

---

## 💡 Key Features

- Developed entirely in **LabVIEW (.vi)**
- Real-time analog signal processing
- Directional motor control logic
- Tolerance threshold for stable stop behavior
- Scalable motor speed based on error magnitude (if included)

---

## 📁 Files

- `Automatic-Control-single-input---single-output.vi`: Main control file
- Optional:
  - `ControlLogicSub.vi`: (if modularized)
  - `DAQConfig.vi`: Handles hardware channels and signal mapping

---

## 📷 Optional Add-ons

- LCD/Graphical output to display current input/output
- Logging system using `.csv` for data analysis
- PID control implementation for smoother and more accurate performance

---

## 🧪 Learning Outcomes

- Application of **feedback control** theory in real-time systems
- Hands-on practice with **LabVIEW VI development**
- Interfacing DAQ hardware with external electronics
- Signal acquisition, processing, and actuation principles

---

## 👤 Developed By

This project was submitted as part of the **Automatic Control** course to explore the dynamics of SISO control systems using **LabVIEW and real-world hardware integration**.

---

