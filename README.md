# Embedded Assistive Device for Alzheimer's Disease Patients

An affordable, reliable, and real-time wearable IoT solution designed to improve patient safety, promote independence, and reduce caregiver burden for individuals living with Alzheimer's disease.

## 📌 Project Overview
Alzheimer's disease is a progressive neurologic disorder that causes memory loss, disorientation, and diminished capacity to carry out activities of daily living. This project introduces an ESP32-based embedded assistive device that tracks a patient's real-time location, monitors vital health parameters, detects physical falls, and provides automated voice reminders for daily medications and routines.

---

## 🚀 Key Features & Modules
The system utilizes a modular design integrated into a central processing framework:

* **Real-Time Location Tracking (NEO-6M GPS):** Continuously tracks geographic coordinates and allows for alerts if a patient wanders.
* **Fall Detection System (MPU-6050):** Utilizes an accelerometer and gyroscope to detect sudden abnormal impacts or orientation shifts, instantly flagging emergency situations.
* **Biometric Monitoring (Pulse & GSR Sensors):** Measures heart rate (BPM) and skin conductivity to evaluate the patient's emotional stress, anxiety, or vitals stability.
* **Automated Voice Reminders (DFPlayer Mini + Speaker):** Plays pre-recorded audio cues reminding patients to take medication or stay hydrated, boosting independence.
* **Central Processor (ESP32 Microcontroller):** Handles low-power multi-sensor data processing and establishes wireless communication baselines.

---

## 🛠️ Hardware Architecture & Specifications

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
The system is built entirely on highly accessible, low-cost components, bringing the total estimated prototype cost to **₹3,300 – ₹3,500 INR**, making it deeply viable for scalable home-care deployment.

---

## 💻 Firmware & Standards Compliance
* **Language & Environment:** C / C++ utilizing the Arduino IDE.
* **Communication Standards:** Built using industrial protocols—**UART** for GPS data transmission, **I2C** for interacting with the MPU-6050 inertial sensor, and standard serial communication for audio control.
* **Safety Profile:** Low-voltage DC powered (rechargeable 5V battery subsystem) ensuring user safety.

---

## 📈 Testing & Results
* **GPS Tracking:** Verified accurate spatial tracking within a 5–10 meter boundary.
* **Fall Sensing:** Successfully registered simulated sudden-impact drops to flag an alert state.
* **Vitals & Stress Monitoring:** Recorded stable resting heart rates (70-90 BPM) and responsive skin conductance alterations under shifting stress parameters.

---

## 🔮 Future Enhancements
* Development of native mobile applications for immediate caregiver push notifications.
* Cloud database integration for long-term physiological data telemetry and modeling.
* Machine Learning (ML) integration for forecasting personalized stress thresholds and predicting cognitive deterioration patterns.

---

## 👥 Developers & Contributors
* **Saravanan S** ([Email](mailto:saravanansankar2917@gmail.com)) — B.Tech Electrical and Electronics Engineering
* **Ranganathan V** — B.Tech Electrical and Electronics Engineering
* **Praveen Kumar P** — B.Tech Electrical and Electronics Engineering
