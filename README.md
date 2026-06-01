# EMBEDDED-DEVICE-FOR-ALZHEIMER-S-DISEASE-PATIENTS
An ESP32-based wearable IoT device for Alzheimer's patients. Integrates NEO-6M GPS for tracking , MPU-6050 for fall detection , and Pulse/GSR sensors for heart rate and stress telemetry. Uses a DFPlayer Mini for automated voice reminders. Programmed in C to create a low-cost (₹3.5k), scalable smart healthcare solution

##  Project Overview
[cite_start]Alzheimer's disease is a progressive neurologic disorder that causes memory loss, disorientation, and diminished capacity to carry out activities of daily living[cite: 283]. [cite_start]This project introduces an ESP32-based embedded assistive device that tracks a patient's real-time location, monitors vital health parameters, detects physical falls, and provides automated voice reminders for daily medications and routines[cite: 284, 285].

---

##  Key Features & Modules
[cite_start]The system utilizes a modular design integrated into a central processing framework[cite: 345, 346]:

* [cite_start]**Real-Time Location Tracking (NEO-6M GPS):** Continuously tracks geographic coordinates and allows for geofencing alerts if a patient wanders[cite: 347, 348].
* [cite_start]**Fall Detection System (MPU-6050):** Utilizes an accelerometer and gyroscope to detect sudden abnormal impacts or orientation shifts, instantly flagging emergency situations[cite: 354, 355].
* [cite_start]**Biometric Monitoring (Pulse & GSR Sensors):** Measures heart rate (BPM) and skin conductivity to evaluate the patient's emotional stress, anxiety, or vitals stability[cite: 351, 357].
* [cite_start]**Automated Voice Reminders (DFPlayer Mini + Speaker):** Plays pre-recorded audio cues reminding patients to take medication or stay hydrated, boosting independence[cite: 359].
* [cite_start]**Central Processor (ESP32 Microcontroller):** Handles low-power multi-sensor data processing and establishes wireless communication baselines[cite: 361, 363].

---

##  Hardware Architecture & Specifications

### Component Technical Breakdown
| Component | Function / Role | Interface Used | Operating Voltage |
| :--- | :--- | :--- | :--- |
| **ESP32** | Core microcontroller & processing unit | GPIO, UART, I²C | 3.3V |
| **NEO-6M GPS** | Real-time position tracking | UART (TX/RX) | 3.3V–5V |
| **Pulse Sensor** | Heart rate tracking via Photoplethysmography | Analog Input | 3.3V |
| **MPU-6050** | Motion tracking (Accelerometer + Gyroscope) | I²C | 3.3V |
| **GSR Sensor** | Galvanic Skin Response (Stress measurement) | Analog Input | 3.3V–5V |
| **DFPlayer Mini** | MP3 Audio playback for voice reminders | Serial | 5V |

### Cost Analysis (Economic Feasibility)
[cite_start]The system is built entirely on highly accessible, low-cost components, bringing the total estimated prototype cost to **₹3,300 – ₹3,500 INR**, making it deeply viable for scalable home-care deployment[cite: 437, 440].

---

## 💻 Firmware & Standards Compliance
* [cite_start]**Language & Environment:** C / C++ utilizing the Arduino IDE[cite: 379].
* [cite_start]**Communication Standards:** Built using industrial protocols—**UART** for GPS data transmission, **I2C** for interacting with the MPU-6050 inertial sensor, and standard serial communication for audio control[cite: 377].
* [cite_start]**Safety Profile:** Low-voltage DC powered (rechargeable 5V battery subsystem) ensuring user safety[cite: 378, 403].

---

## 📈 Testing & Results
* [cite_start]**GPS Tracking:** Verified accurate spatial tracking within a 5–10 meter boundary[cite: 425].
* [cite_start]**Fall Sensing:** Successfully registered simulated sudden-impact drops to flag an alert state[cite: 429].
* [cite_start]**Vitals & Stress Monitoring:** Recorded stable resting heart rates (70-90 BPM) and responsive skin conductance alterations under shifting stress parameters[cite: 417, 430].

---

## 🔮 Future Enhancements
* [cite_start]Development of native mobile applications for immediate caregiver push notifications[cite: 446].
* [cite_start]Cloud database integration for long-term physiological data telemetry and modeling[cite: 446].
* [cite_start]Machine Learning (ML) integration for forecasting personalized stress thresholds and predicting cognitive deterioration patterns[cite: 331, 447].

---

## 👥 Developers & Contributors
* [cite_start]**Saravanan S** ([Email](mailto:saravanansankar2917@gmail.com)) — B.Tech Electrical and Electronics Engineering[cite: 467].
* [cite_start]**Ranganathan V** — B.Tech Electrical and Electronics Engineering[cite: 467].
* [cite_start]**Praveen Kumar P** — B.Tech Electrical and Electronics Engineering[cite: 468].
