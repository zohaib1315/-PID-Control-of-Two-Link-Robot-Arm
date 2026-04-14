# -PID-Control-of-Two-Link-Robot-Arm
This project implements a **PID-based control system** for a nonlinear **two-link robotic manipulator** using MATLAB, Simulink, and Simscape Multibody.  The objective is to achieve accurate trajectory tracking of joint angles under different control strategies (P, PD, PID) and evaluate their performance.
---

## ⚙️ System Model

The robot dynamics are governed by:

M(q)q̈ + V(q, q̇) + G(q) = τ

Where:
- q = joint angles
- M(q) = inertia matrix
- V(q, q̇) = Coriolis and centrifugal forces
- G(q) = gravitational torque
- τ = control input (joint torques)

---

## 🏗️ Implementation

- Built a **2-DOF robotic arm** using Simscape Multibody
- Configured:
  - Revolute joints with torque actuation
  - Rigid body links
  - Sensor feedback for joint angles
- Designed **independent joint controllers** (decentralized control)

---

## 🎯 Controllers Implemented

- **P Controller**
- **PD Controller**
- **PID Controller**

Each controller was tested for:
- Step input
- Square wave reference tracking

---

## 📊 Results

| Controller | Behavior |
|----------|--------|
| P | Fast response but high oscillations |
| PD | Improved damping, reduced overshoot |
| PID | Best performance with minimal steady-state error |

✔ PID controller achieved:
- Accurate tracking  
- Reduced oscillations  
- Improved stability  

---

## 🧠 Key Concepts

- Nonlinear robotic dynamics
- Decentralized joint control
- Feedback control systems
- Simscape Multibody modeling
- PID tuning and performance evaluation

---

## 🛠️ Tools & Technologies

- MATLAB
- Simulink
- Simscape Multibody

---

## 📷 Simulation Model

*(Add your Simulink diagram screenshot here)*

---

## 🚀 How to Run

1. Open MATLAB
2. Load the `.slx` file
3. Run simulation
4. Modify controller gains (Kp, Ki, Kd) to observe behavior

---

## 📌 Future Improvements

- Computed torque control (nonlinear control)
- Adaptive PID tuning
- Trajectory planning (circular/complex paths)
- Real-time hardware implementation

---

## 👨‍💻 Author

Zohaib Ahmed Mughal  
Electrical Engineering Student  
[LinkedIn](https://linkedin.com/in/zohaib-mughal-43321a325)  
[GitHub](https://github.com/zohaib1315)
