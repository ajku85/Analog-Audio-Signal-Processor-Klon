
# Analog Signal Processor: Klon Centaur Clone (Manufacturing & Analysis)

## Project Overview
This project documents the end-to-end assembly, quality control, and technical analysis of a high-fidelity analog audio signal processor based on the Klon Centaur circuit. The objective was to execute a reliable **Through-Hole Technology (THT) assembly process** following a strict Control Plan and Design for Manufacturing (DFM) principles.

## 1. Engineering & Design
*(See `/01_Engineering_Design` for schematics, layout, and mechanical drawings)*

The device features specific analog design choices validated during the build:

* **Power Management:** Implementation of a **Charge Pump (ICL7660S)** voltage converter. This boosts the standard +9V input to a ~18V internal rail, providing greater dynamic headroom and preventing unwanted distortion in the Op-Amp buffer stages.
* **Non-Linear Response:** Usage of **Germanium Diodes (1N34A)** in the feedback loop for specific "soft-clipping" signal conditioning, distinct from silicon-based hard clipping.
* **Mechanical Design:** Enclosure drilling template designed to ensure precise alignment of potentiometers and jacks.
    * *File Ref:* `3_Mechanical_Enclosure/Enclosure_Drill_Template.png`

## 2. Manufacturing Process Log
*(See `/02_Manufacturing_Log` for visual progression)*

The assembly followed a sequential workflow to minimize defects. Key milestones documented:

### Phase 1: Incoming Inspection & BOM Verification
* **File:** `01_Incoming_Parts_Check.jpg` & `02_Components_Detail.jpg`
* **Action:** Verified raw components against the Bill of Materials (BOM). Checked resistor values (1% Metal Film) using a multimeter and verified capacitor tolerances before acceptance.

### Phase 2: THT Assembly (PCBA)
* **File:** `03_THT_Assembly_Stage1.jpg`
* **Action:** Populated low-profile components first (Resistors/Diodes) followed by IC sockets.
* **File:** `04_PCBA_Completed_Top.jpg`
* **Action:** Completed board assembly. Visual inspection of solder joints to ensure proper wetting and absence of cold joints or solder bridges.

### Phase 3: Final Integration & Wiring
* **File:** `05_Final
