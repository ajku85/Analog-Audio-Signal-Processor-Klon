# Analog Signal Processor: Klon Centaur Clone (Manufacturing & Analysis)

## Project Overview
This project documents the end-to-end assembly, quality control, and technical analysis of a high-fidelity analog audio signal processor based on the Klon Centaur circuit. The objective was to execute a reliable **Through-Hole Technology (THT) assembly process** following a strict Control Plan.

> **Project Scope Note:**
> This project was executed in two parallel streams to maximize learning outcomes:
> 1. **Design & Analysis:** The circuit schematics and PCB layout were designed/modeled in **EasyEDA** to study the topology and signal paths.
> 2. **Physical Implementation:** The physical assembly utilized a **standardized component kit** to focus strictly on **THT soldering quality, process control, and FMEA execution**, ensuring a reliable reference for testing.

---

## 1. Engineering Design
*(Technical Documentation & Schematics)*

### Circuit Diagram
Analysis of the dual-ganged summing amplifier topology and charge pump power supply (+18V).
![Schematic Diagram](KlonCentaurProject/01_Engineering_Design/1_Schematics/Circuit_Diagram_Rev1.png)

### PCB Layout (Top Layer)
Design optimized for signal integrity and low noise floor.
![PCB Top Layer](KlonCentaurProject/01_Engineering_Design/2_PCB_Layout/PCB_Top_Layer.png)

---

## 2. Manufacturing Process Log
*(Visual documentation of the THT assembly workflow)*

### THT Assembly Phase (PCBA)
Populating low-profile components (Resistors/Diodes) and IC sockets.
![Assembly Stage](KlonCentaurProject/02_Manufacturing_Log/03_THT_Assembly_Stage1.jpg)

### Final Integration & Wiring
Internal view showing off-board wiring, star-grounding implementation, and mechanical assembly.
![Internal Wiring](KlonCentaurProject/02_Manufacturing_Log/05_Final_Internal_Wiring.jpg)

### Final Product
Completed unit ready for Functional Testing (FNT).
![Final Product](KlonCentaurProject/02_Manufacturing_Log/06_Final_Product_Exterior.jpg)

---

## 3. Quality Assurance: FMEA Approach
A **Failure Mode and Effect Analysis (FMEA)** was conducted to anticipate assembly risks (Excerpt from project documentation):

| Process Step | Potential Failure Mode | Risk Priority (RPN) | Mitigation Strategy |
| :--- | :--- | :--- | :--- |
| **Component Insertion** | Polarized Capacitor Reverse | High (81) | Verify stripe orientation before soldering; QC check. |
| **Soldering** | Solder Bridge (Short Circuit) | Medium (64) | Post-solder visual inspection & Flux cleaning. |
| **Wiring** | DC Jack Polarity Inversion | Low (18) | Continuity test with multimeter before powering up. |

---

## Tools & Equipment Used
* **Soldering:** Adjustable Temperature Station (350°C).
* **Measurement:** Digital Multimeter (Continuity, Resistance, Voltage drop).
* **Documentation:** EasyEDA (Schematics), MS Word (Process Flowchart).

---
*Project executed by Andres Guevara Gamboa - University of Pécs*
