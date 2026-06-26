# ⚡ DC-DC Buck Converter using TL494

> **Power Electronics Laboratory Project**  
> **Indian Institute of Technology (IIT) Indore**

---

## 📖 Overview

This repository presents the complete design, implementation, and experimental analysis of a **Non-Isolated DC-DC Buck Converter** using the **TL494 PWM Controller IC**. The project demonstrates the practical realization of a high-efficiency step-down converter and its operation under both **Continuous Conduction Mode (CCM)** and **Discontinuous Conduction Mode (DCM)**.

The converter was designed, assembled, and experimentally validated using oscilloscope measurements and hardware testing.

---

## 🎯 Objective

The objectives of this project are:

- Design and implement a DC-DC Buck Converter using the TL494 PWM controller.
- Convert a **20 V DC input** to a regulated **7.5 V DC output**.
- Generate PWM pulses for MOSFET switching.
- Analyze converter performance in Continuous Conduction Mode (CCM).
- Demonstrate Discontinuous Conduction Mode (DCM) by reducing the switching frequency.
- Observe and analyze the inductor current and switch voltage waveforms.

---

## ⚙️ Specifications

| Parameter | Value |
|-----------|-------|
| Input Voltage (Vin) | 20 V |
| Output Voltage (Vout) | 7.5 V |
| Switching Frequency | 20 kHz |
| Output Current | 1 A |
| PWM Controller | TL494 |
| Converter Type | Non-Isolated Buck Converter |

---

## 🛠 Hardware Components

- TL494 PWM Controller IC
- MOSFET Power Switch
- Gate Driver Circuit
- Power Inductor
- Freewheeling Diode
- Output Capacitor
- PCB
- Oscilloscope
- DC Power Supply
- Resistive Load

---

## 🧠 Working Principle

A Buck Converter is a switched-mode DC-DC converter that reduces a higher DC input voltage to a lower regulated output voltage.

The TL494 PWM controller generates switching pulses that drive the MOSFET. During the ON period, energy is stored in the inductor. During the OFF period, the stored energy is transferred to the load through the freewheeling diode.

The ideal voltage conversion relationship is:

\[
V_{out}=D\times V_{in}
\]

where

- **D** = Duty Cycle
- **Vin** = Input Voltage
- **Vout** = Output Voltage

---

## 🔄 Converter Operation

### MOSFET ON

- MOSFET conducts.
- Inductor stores energy.
- Diode remains reverse biased.
- Load receives power through the output capacitor.

### MOSFET OFF

- MOSFET turns OFF.
- Inductor releases stored energy.
- Current flows through the freewheeling diode.
- Capacitor smooths the output voltage.

---

## 📊 Experimental Results

### (a) Continuous Conduction Mode (CCM)

**Operating Conditions**

- Input Voltage = **20 V**
- Output Voltage = **6.3 V**
- Output Current = **1 A**
- Switching Frequency = **20.7 kHz**

**Waveforms Observed**

- Inductor Current
- Switch Voltage

**Measured Values**

- Average Switch Voltage = **17.87 V**
- Average Inductor Current = **970 mA**

The inductor current remains above zero throughout the switching cycle, confirming Continuous Conduction Mode (CCM).

---

### (b) Discontinuous Conduction Mode (DCM)

To demonstrate DCM, the switching frequency was reduced.

**Operating Conditions**

- Output Voltage = **8.65 V**
- Switching Frequency = **6.5 kHz**

**Waveforms Observed**

- Inductor Current
- Switch Voltage

**Measured Values**

- Average Switch Voltage = **15.20 V**
- Average Inductor Current = **1.8 A**

The inductor current falls to zero before the beginning of the next switching cycle, confirming Discontinuous Conduction Mode (DCM).

---

## 📂 Repository Structure

```
DC-DC-Buck-Converter
│
├── README.md
├── Buck_Converter.pdf
├── Driver.jpeg.zip
├── Converter.jpeg.zip
├── Images/
└── Documentation/
```

---

## 📸 Repository Contents

This repository includes:

- 📄 Complete Project Report
- 📷 Hardware Images
- 📈 CCM Waveforms
- 📈 DCM Waveforms
- ⚡ Gate Driver PCB
- 🔧 Buck Converter Hardware

---

## 🎓 Learning Outcomes

Through this project, the following concepts were studied and implemented:

- DC-DC Buck Converter Design
- PWM Generation using TL494
- MOSFET Switching
- Gate Driver Design
- Continuous Conduction Mode (CCM)
- Discontinuous Conduction Mode (DCM)
- Oscilloscope Measurements
- Hardware Debugging
- Power Electronics Laboratory Techniques

---

## 🚀 Future Improvements

- Closed-loop voltage regulation
- Digital PWM control using microcontrollers
- Improved PCB layout
- Higher efficiency MOSFET driver
- Output voltage feedback control
- Overcurrent and overvoltage protection

---

## 👥 Team Members

- Parekh Om Nirav
- Praharsha Sandineni
- Siddhartha Porika
- Yash Brijesh Modi

**Department of Electrical Engineering**

**Indian Institute of Technology Indore**

---

## 📄 Documentation

The repository contains the complete project report, hardware photographs, oscilloscope waveforms, and supporting documentation related to the design and implementation of the DC-DC Buck Converter.

---

## 📜 Conclusion

The DC-DC Buck Converter using the TL494 PWM Controller was successfully designed, implemented, and tested. Experimental observations under both Continuous Conduction Mode (CCM) and Discontinuous Conduction Mode (DCM) closely matched the expected theoretical behavior, validating the converter design and demonstrating practical concepts of switching power electronics.

---

⭐ **If you found this project useful, consider giving this repository a star!**
