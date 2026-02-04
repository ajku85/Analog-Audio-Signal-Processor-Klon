# Analog Signal Processor: Klon Centaur Clone

## Project Overview
This project involves the assembly, analysis, and verification of a high-fidelity analog audio signal processor based on the legendary Klon Centaur circuit. The goal was to study **signal integrity**, **non-linear amplification (clipping)**, and **power supply charge pumps** in a practical audio application.

## Technical Highlights
* **Circuit Topology:** Overdrive circuit with a unique "dual-ganged" gain potentiometer that blends the clean signal with the clipped signal (Summing Amplifier).
* **Clipping Mechanism:** Utilizes **Germanium Diodes (1N34A)** for soft-clipping characteristics, distinct from the hard-clipping found in silicon-based circuits.
* **Power Management:** Includes a **Charge Pump (ICL7660S)** to convert +9V input into +18V internal headroom, increasing dynamic range and preventing unwanted distortion in the buffer stage.
* **Impedance Matching:** High-impedance JFET Input Buffer to prevent signal loading (Tone Sucking).

## Verification & Measurements
*(See `/Measurements` folder for oscilloscope screenshots)*

To validate the circuit's performance, I conducted physical tests using a standard Oscilloscope and Function Generator:

* **Test Signal:** 1 kHz Sine Wave, 500mVpp.
* **Clipping Analysis:** Verified the "Soft Clipping" behavior. Unlike the square-wave cutoff typical of Silicon diodes (0.7V drop), the Germanium diodes (0.3V drop) produced a rounded compression of the sine wave peaks, confirming the desired harmonic distortion profile.
* **Output Buffer:** Verified unity gain and signal stability at the output stage.

## Build Quality
*(See `/Build_Photos` folder)*

* **Soldering:** Through-hole (THT) assembly with focus on joint reliability and flux cleaning.
* **Wiring:** Star-grounding technique used to minimize 50Hz/60Hz hum and chassis noise.
* **Components:** Metal film resistors (1% tolerance) used in signal paths to reduce thermal noise.

## Tools Used
* **Hardware:** Soldering Station, Digital Multimeter, Oscilloscope.
* **Software:** LTspice (for preliminary simulation), KiCad (schematic review).

---
*Author: Andres Guevara Gamboa*
