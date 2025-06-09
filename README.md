# 🚀 HoverCraft 290

## 📌 About the Project
**HoverCraft 290** is a fully autonomous hovercraft designed to navigate through a track with obstacles and turns. It uses sensor fusion and real-time control logic written in **Pure C for AVR microcontrollers** to stabilize, detect, and maneuver dynamically.

![Image](https://github.com/user-attachments/assets/14433d42-9568-49f8-953d-2b6cb394bbae)
---

## ✨ Features & Components

### 🔧 Technologies Used
- **Programming Language:** Pure C (AVR-GCC)
- **Microcontroller Platform:** Arduino Nano (ATmega328P)
- **Control Techniques:** PID control for yaw stabilization, PWM for fans and servo

### 📡 Sensors Used
- **Ultrasonic Sensor (HC-SR04):** Measures distances and detects nearby obstacles
- **IR Analog Rangefinder (GP2Y0A21):** Detects endpoint via overhead bar
- **IMU (MPU-6050 Gyroscope & Accelerometer):** Provides orientation (yaw) for stable turning

### ⚙️ Actuators & Hardware
- **Lift Fan (AFB1212SH):** Enables the hovercraft to float
- **Propulsion Fan (MEC0251V1-0000-A99):** Provides forward thrust
- **Servo Motor (HS-311):** Dynamically redirects propulsion based on turning logic
- **Battery:** Rhino 460 2S 20C for stable high-discharge power

---

## 🎥 Demonstration GIFs

|  1️⃣ Hovercraft Lifting All Components |
|---------------------------------------|
| ![Hover Lift](https://github.com/FabioKoshy/HoverCraft-290-/blob/main/Hovering%20.gif) |

|  2️⃣ Trial Run | 3️⃣ Resilient Impact |
|------------------|------------------------|
| ![Maze Navigation](https://github.com/FabioKoshy/HoverCraft-290-/blob/main/Hovercraft%20demo.gif) | ![Hovers over objects](https://github.com/FabioKoshy/HoverCraft-290-/blob/main/Resilient%20impact.gif) |

|  4️⃣ Base Build                         |
|-------------------------------------------|
| ![Base Build](https://github.com/FabioKoshy/HoverCraft-290-/blob/main/Base%20Build.jpg) |

---

## 📄 Full Technical Report

For detailed documentation of design decisions, component integration, results, and evaluation:
👉 [Download ENGR 290 Final Report (PDF)](https://github.com/FabioKoshy/HoverCraft-290-/blob/main/ENGR%20290%20FALL%202024%20Project%20Team2.pdf)

---

## 📝 Additional Notes
- The hovercraft uses PID control to adjust the servo angle based on IMU yaw readings.
- The system dynamically chooses to turn left or right depending on which path is longer, as detected by the ultrasonic sensor rotating via the servo.
- The IR sensor detects an overhead bar to trigger shutdown at the track endpoint.

---

