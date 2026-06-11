# 👕 Automatic Clothes Segregator

> An Arduino-based automated clothes sorting system that uses a TCS3200 Color Sensor and Servo Motors to classify garments into separate compartments based on their color, reducing manual effort and preventing color mixing during washing.

![Arduino](https://img.shields.io/badge/Arduino-Nano-blue)
![Sensor](https://img.shields.io/badge/Sensor-TCS3200-green)
![Automation](https://img.shields.io/badge/Domain-Industrial_Automation-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 📖 Overview

Sorting white and colored clothes before washing is a repetitive and time-consuming task. Mixing garments of different colors may result in color bleeding, fading, and fabric damage.

The **Automatic Clothes Segregator** is an embedded automation project that identifies garment color using a **TCS3200 Color Sensor** and automatically directs the cloth into the appropriate compartment using **servo motors** controlled by an **Arduino Nano/Uno**.

This project demonstrates how low-cost sensors and microcontrollers can be integrated to automate sorting operations in laundry services, garment manufacturing, and textile industries.

---

## 🎯 Objectives

- Automate the process of clothes segregation.
- Reduce human effort in laundry operations.
- Prevent color mixing during washing.
- Improve sorting efficiency and accuracy.
- Demonstrate practical applications of embedded systems and sensor interfacing.

---

## ✨ Features

- Automatic color detection using TCS3200 sensor
- Servo-based cloth transportation and sorting
- Arduino-controlled decision making
- Real-time classification of garments
- Compact and low-cost hardware design
- Suitable for educational and industrial automation applications

---

## 🛠 Hardware Components

| Component | Quantity |
|------------|------------|
| Arduino Nano / Uno | 1 |
| TCS3200 Color Sensor | 1 |
| Servo Motor (SG90) | 2 |
| 5V Power Supply | 1 |
| Sorting Compartments | 2 |
| Connecting Wires | As Required |

---

## 💻 Software Requirements

- Arduino IDE
- Embedded C Programming
- Servo Library
- TCS3200 Sensor Interface Code

---

## ⚙️ System Workflow

1. A cloth is placed at the input section.
2. Servo Motor 1 moves the cloth beneath the color sensor.
3. The TCS3200 sensor detects the cloth color.
4. The sensor output is processed by the Arduino Nano.
5. The controller compares the detected values with predefined thresholds.
6. Servo Motor 2 rotates accordingly.
7. The cloth is directed into:
   - Compartment 1 → White Clothes
   - Compartment 2 → Colored Clothes

---

## 🏗 System Architecture

```text
Input Clothes
      │
      ▼
 Servo Motor 1
      │
      ▼
 TCS3200 Color Sensor
      │
      ▼
 Arduino Nano/Uno
      │
      ▼
 Servo Motor 2
      │
 ┌────┴────┐
 ▼         ▼
White     Colored
Bin        Bin
```

---

## 📊 Block Diagram

![Block Diagram](images/ACS_Block_Diagram.PNG)

---

## 🔌 Circuit Diagram

![Circuit Diagram](images/ACS_Ckt_Diagram.jpeg)

---

## 🔧 Hardware Setup

![Hardware Setup](images/ACS_CKT_Design.jpeg)

---

## 🔗 Circuit Connections

### TCS3200 Sensor Connections

| TCS3200 Pin | Arduino Pin |
|------------|------------|
| VCC | 5V |
| GND | GND |
| S0 | D2 |
| S1 | D3 |
| S2 | D4 |
| S3 | D5 |
| OUT | D6 |

### Servo Motor Connections

| Servo Pin | Arduino Pin |
|------------|------------|
| Servo 1 Signal | D7 |
| Servo 2 Signal | D8 |
| VCC | 5V |
| GND | GND |

---

## 🧠 Working Principle

The TCS3200 Color Sensor consists of an array of photodiodes with red, green, blue, and clear filters. When a garment is placed below the sensor, reflected light is converted into frequency signals corresponding to RGB values.

The Arduino Nano reads these values and determines whether the cloth belongs to the white category or colored category. Based on this decision, Servo Motor 2 rotates to guide the cloth into the appropriate compartment.

This process is fully automated and requires minimal human intervention.

---

## 📈 Results

The prototype was tested on 100 clothing samples under controlled conditions.

| Parameter | Value |
|------------|------------|
| Color Detection Accuracy | 95% |
| Reliability | 95% |
| Measurement Range | 100% Visible Spectrum |
| Calibration Requirement | Periodic |

### Key Outcomes

✅ Accurate segregation of white and colored garments

✅ Reduced manual sorting effort

✅ Reliable operation in controlled lighting conditions

✅ Low-cost and scalable implementation

---

## 🚀 Applications

- Smart Laundry Systems
- Textile Manufacturing Industries
- Garment Processing Units
- Retail Clothing Sorting
- Automated Warehousing
- Industrial Automation Systems

---

## 📚 Research Publication

### Automatic Clothes Segregator

**Authors**

- Suvarna Kadam
- Sanika Deshpande
- Varsha Bendre
- Yash Dhond
- Rashmi Patil
- Anuj Gavhane

This project was developed as an academic research initiative focusing on color-based automated garment segregation using embedded systems and sensor technologies.

---

## 🔮 Future Enhancements

- Multi-color classification
- Fabric type identification
- Conveyor belt integration
- Camera-based computer vision system
- Machine Learning based color recognition
- Mobile application monitoring
- Cloud-based analytics dashboard

---

## 📁 Repository Structure

```text
Automatic_Clothes_Segregator/
│
├── README.md
│
├── docs/
│   └── ACS_Research_Paper.pdf
│
├── images/
│   ├── ACS_Block_Diagram.PNG
│   ├── ACS_CKT_Design.jpeg
│   ├── ACS_Ckt_Diagram.jpeg
│   └── Prototype.jpg
│
├── code/
│   └── Automatic_Clothes_Segregator.ino
│
├── hardware/
│   ├── Circuit_Diagram.pdf
│   └── Bill_of_Materials.xlsx
│
└── LICENSE
```

---

## 🧰 Technologies Used

- Embedded C
- Arduino IDE
- Arduino Nano / Uno
- TCS3200 Color Sensor
- Servo Motor Control
- PWM Signal Generation
- Sensor Interfacing
- Embedded System Design

---

## 📌 Key Learning Outcomes

- Embedded System Design
- Sensor Interfacing
- Arduino Programming
- Automation Techniques
- Servo Motor Control
- Hardware-Software Integration
- Prototype Development
- Technical Documentation

---

## 👨‍💻 Author

### Anuj Gavhane

Electronics & Telecommunication Engineer

**Areas of Interest**

- Embedded Systems
- Firmware Development
- Industrial Automation
- IoT Solutions
- Automotive Electronics
- Robotics

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

Feedback, suggestions, and contributions are always welcome!

---
