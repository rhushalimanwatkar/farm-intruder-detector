# Farm-Intruder-Detector-System


An analog electronic security alarm designed to protect farmland, crops, and livestock from unauthorized entry or animal intrusions. Utilizing a **Passive Infrared (PIR) Motion Sensor** connected to a **BC547 NPN transistor**, the system detects motion in real-time and triggers a visual (**LED**) and audible (**Buzzer**) alert.

---

## 🛠️ Components List

| Component | Description / Specification | Quantity |
| :--- | :--- | :---: |
| **PIR Sensor** | HC-SR501 Passive Infrared Motion Sensor | 1 |
| **NPN Transistor** | BC547 (Solid-state switch / Amplifier) | 1 |
| **Buzzer** | 9V Piezo Electric Buzzer (Audible Alarm) | 1 |
| **LED** | 5mm LED (Visual Indicator) | 1 |
| **Resistors** | 1kΩ   | 3 |
| **Power Source** | 9V DC Battery / Power Supply | 1 |
| **Breadboard & Wires** | Jumper Wires and Prototyping Board | — |

---

## ⚙️ Working Principle

1. **Standby Mode (No Motion):**
   * The **PIR Sensor** continuously monitors the infrared thermal radiation in its field of view.
   * When no human or animal motion is detected, the PIR sensor output pin remains **LOW (0V)**.
   * The **BC547 transistor** receives no base current and remains **OFF**, keeping both the LED and Buzzer turned **OFF**.

2. **Alert Triggered (Motion Detected):**
   * When a intruder or animal enters the detection zone, the PIR sensor registers the change in infrared levels and sets its output pin to **HIGH (~3.3V)**.
   * This HIGH signal delivers current to the base of the **BC547 transistor**, switching it into **saturation (ON state)**.
   * Current flows from collector to emitter, completing the circuit to sound the **Buzzer** and illuminate the **LED** simultaneously.

---

## 🔌 Project Implementation

The project was developed in two main phases:
1. **Breadboard Prototyping:** The initial circuit was built and tested on a breadboard using a 9V power supply, PIR sensor, BC547 transistor, buzzer, and LED to verify component behavior, sensitivity, and switching logic.
2. **PCB Implementation:** Once the analog logic and trigger responses were successfully verified, the circuit was soldered onto a permanent PCB for a stable, compact, and robust final deployment.

---

## 📄 Project Documentation & Report

For detailed schematic diagrams,and hardware explanations, refer to the project documentation:
[Farm-Intruder-Detector_Mini_Project_Report.pdf](https://github.com/user-attachments/files/34618765/Farm-Intruder-Detector_Mini_Project_Report.pdf)

---
