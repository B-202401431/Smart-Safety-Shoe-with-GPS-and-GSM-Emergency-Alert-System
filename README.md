# 👟 Smart Safety Shoe with GPS and GSM Emergency Alert System

A wearable safety device designed to improve women's safety by providing instant emergency alerts with GPS location tracking and a built-in self-defense mechanism.

---

# 📖 Overview

The **Smart Safety Shoe** is an ESP32-based wearable safety system that helps users during emergency situations. By pressing the panic button mounted on the side of the shoe, the system automatically retrieves the user's current GPS location and sends an SMS containing the location to predefined emergency contacts using the GSM network.

The shoe also includes a self-defense shock module that can be activated during emergencies.

> **Note**
>
> The original project proposal included a **wireless panic button wristband**.
> In the final implemented prototype, the **panic button is directly mounted on the shoe** instead of using a wireless wristband. This modification improves reliability and simplifies the overall hardware design.

---

# 📷 Project Images

## Complete Smart Safety Shoe

![Smart Safety Shoe](IMG_20251126_190008.jpg)

---

## Internal Electronics

![Internal Electronics](IMG_20251126_185907.jpg)

---

## Internal Prototype

![Prototype](IMG_20251126_190017.jpg)

---

# 🎥 Project Demonstration

Watch the complete working demonstration here:

**Google Drive Link**

```
Paste Your Google Drive Video Link Here
```

---

# 🚨 Features

- Emergency panic button
- Live GPS location tracking
- GSM SMS alert system
- ESP32 microcontroller
- Rechargeable battery
- Built-in self-defense shock module
- Compact wearable design
- Portable embedded system

---

# ⚙️ Hardware Components

| Component | Description |
|------------|-------------|
| ESP32 Dev Board | Main Controller |
| SIM800L GSM Module | Sends Emergency SMS |
| NEO-6M GPS Module | Retrieves Live GPS Coordinates |
| Shock Module | Self-defense mechanism |
| Relay Driver | Controls Shock Module |
| 2 × 18650 Li-ion Batteries | Power Supply |
| TP4056 Charging Module | Battery Charging |
| Panic Push Button | Emergency Trigger |
| Conductive Plates | Shock Output |
| Power Switch | Main ON/OFF Control |

---

# 🔄 Working Principle

1. User presses the panic button mounted on the shoe.

2. ESP32 detects the button press.

3. ESP32 communicates with the NEO-6M GPS module to obtain the current latitude and longitude.

4. The SIM800L GSM module sends an SMS containing the GPS location to predefined emergency contacts.

5. Simultaneously, the ESP32 activates the relay to enable the shock module for self-defense.

---

# 🖥 System Architecture

```
              Panic Button
                    │
                    ▼
                 ESP32
          ┌─────────┴─────────┐
          │                   │
          ▼                   ▼
    GPS Module          GSM Module
          │                   │
          │             Sends SMS Alert
          ▼
   Live Coordinates
          │
          ▼
      Relay Driver
          │
          ▼
     Shock Module
          │
          ▼
   Conductive Plates
```

---

# 📱 SMS Format

Example emergency SMS:

```
Emergency!

I need immediate help.

My Current Location

Latitude : XX.XXXXXX

Longitude : YY.YYYYYY

Google Maps

https://maps.google.com/?q=latitude,longitude
```

---

# 🔋 Power Supply

The system is powered using:

- Two 3.7V Rechargeable 18650 Li-ion Batteries
- TP4056 Charging Module
- Slide ON/OFF Switch

---

# 💻 Software

- Arduino IDE
- ESP32 Board Package
- TinyGPS++
- SoftwareSerial
- SIM800L AT Commands

---

# 📁 Repository Structure

```
Smart-Safety-Shoe-with-GPS-and-GSM-Emergency-Alert-System/

│
├── README.md
├── LICENSE
├── report.pdf
├── IMG_20251126_185907.jpg
├── IMG_20251126_190008.jpg
└── IMG_20251126_190017.jpg
```

---

# 📊 Project Specifications

| Parameter | Value |
|-----------|-------|
| Controller | ESP32 |
| GPS | NEO-6M |
| GSM | SIM800L |
| Battery | 2 × 18650 Li-ion |
| Charging | TP4056 |
| Communication | GSM SMS |
| Tracking | GPS |
| User Input | Panic Button |
| Output | Shock Module |

---

# 💰 Estimated Cost

| Component | Cost (INR) |
|------------|-----------|
| ESP32 | ₹498 |
| SIM800L | ₹350 |
| NEO-6M GPS | ₹517 |
| Shock Module | ₹300 |
| Relay Module | ₹120 |
| Batteries | ₹800 |
| TP4056 | ₹119 |
| Push Button | ₹20 |
| Conductive Plates | ₹50 |
| Plastic Enclosure | ₹100 |
| Miscellaneous | ₹226 |

## **Total Cost ≈ ₹3100**

---

# ⚠ Disclaimer

This project is developed for educational and research purposes only.

The self-defense shock module must be used responsibly and only where legally permitted. Users must comply with all applicable laws and safety regulations.

---

# 👨‍💻 Team Members

- **Chandan Luhar** (202401431)
- **Krish Hitendrakumar Paghadar** (202401429)
- **Jay Limbasiya** (202401430)
- **Dev Maradiya** (202401432)
- **Dhruvkumar Mistri** (202401433)

### Mentor

**Saurabh Tiwari**

### Course

**PC122**

---

# 📄 Project Report

The complete project report is available here:

[📘 Project Report](report.pdf)

---

# 📚 Reference

This project is inspired by:

**Design of Smart Shoe for Women Safety with Emergency Alert System**

IEEE Xplore Digital Library

The proposed idea was modified and implemented as a practical prototype with the panic button integrated directly into the shoe.
