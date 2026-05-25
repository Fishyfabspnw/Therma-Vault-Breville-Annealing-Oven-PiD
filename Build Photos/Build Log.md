
# ThermaVault PID — Build Log

## Overview

This document tracks the progression of the ThermaVault PID annealing oven conversion project.

The purpose of this build log is to document major design changes, thermal modifications, wiring improvements, and hardware integration throughout the development process.

The project is centered around converting a Breville convection oven into a more stable and serviceable PID-controlled process oven for annealing engineering plastics.

---

# Factory Control Panel Removal

The original Breville front control panel assembly was removed early in the build process to allow integration of a dedicated industrial PID controller and externalized control hardware.

The factory faceplate was retained  during the tear down phase to be repurposed into a new faceplate.
<p align="center">
  <img width="420" alt="Factory control panel" src="https://github.com/user-attachments/assets/0ee69a7e-09fd-4fe2-8b7a-6b8b25b1fa56" />
</p>

---

# Chamber Sealing and Thermal Preparation

High-temperature RTV sealant was applied around exposed seams and panel joints to reduce uncontrolled airflow leakage and improve thermal retention.

Additional ceramic insulation was added around exposed cavities and structural gaps throughout the chamber shell.

Particular attention was given to:

- Heater compartment gaps
- Rear panel seams
- Wire pass-through locations
- Structural openings around the shell

The goal of this stage was to improve chamber consistency and reduce unnecessary heat loss.

<p align="center">
  <img width="700" alt="RTV sealing process" src="https://github.com/user-attachments/assets/08e5e3ac-f2bf-45b4-82d4-6aeea8935a03" />
</p>

<p align="center">
<i>Initial chamber sealing and ceramic insulation integration around exposed shell gaps and rear panel seams.</i>
</p>

<p align="center">
  <img width="700" alt="Upper heater sealing" src="https://github.com/user-attachments/assets/f999d4be-4f12-48a8-b5d0-ff604c824356" />
</p>

<p align="center">
<i>Additional RTV sealing work performed around upper heater routing and structural panel seams.</i>
</p>

---

## Sensor Routing

The RTD PT100 probe was routed through the factory wire pass-through location using a 1/8" NPT compression fitting. This kept the sensor installation clean while avoiding the need for additional holes in the oven chassis.

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/cac5710c-9792-4d3d-9450-c5601a9212b5"
    alt="ThermaVault PT100 sensor routing"
    width="500">
</p>

<p align="center">
  <em>PT100 RTD routing through the factory chassis pass-through using high-temperature sleeving and a 1/8&quot; NPT fitting.</em>
</p>

---

---

# DIN Rail and Wiring Distribution

A compact DIN rail assembly was added to improve wiring organization and modularity.

WAGO lever connectors were mounted using DIN rail carrier adapters to create a cleaner and more serviceable wiring distribution layout.

Compared to direct point-to-point splicing, the DIN rail layout significantly improves:

- Wiring organization
- Future expandability
- Service access
- Troubleshooting capability
- Component replacement simplicity

The terminal distribution layout was designed to keep the wiring compact while maintaining separation between different circuit groups.


<p align="center">
<i>Initial DIN rail and WAGO terminal distribution layout integrated into the rear electronics area.</i>
</p>

<p align="center">
  <img width="700" alt="Updated wiring distribution" src="https://github.com/user-attachments/assets/f27c0409-fb7f-4a93-b142-7d47ae830dd2" />
</p>

<p align="center">
<i>Refined wiring layout with improved routing organization and terminal distribution structure.</i>
</p>


---

## Custom Faceplate Development

A custom replacement faceplate was designed and fabricated to integrate the industrial PID controller and external power controls into a cleaner and more serviceable layout.

The redesigned panel relocates critical process controls outside the primary heated cavity while replacing the original consumer appliance interface with a more industrial control system architecture.

The faceplate assembly was CAD-modeled around the factory oven chassis geometry, existing mounting locations, and component clearance constraints.

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/5f6a2c17-b882-4aa1-8075-845773b2fdbe"
    alt="ThermaVault faceplate CAD front view"
    width="700">
</p>

<p align="center">
  <em>Initial CAD layout for the custom ThermaVault PID control faceplate.</em>
</p>

<br>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/f124674c-6264-40a4-bfa8-d8dfe4d01fb7"
    alt="ThermaVault faceplate CAD secondary view"
    width="500">
</p>

<p align="center">
  <em>CAD development showing controller positioning, switch integration, and chassis fitment planning.</em>
</p>

---

## Convection Fan Calibration

During initial testing, the factory convection fan assembly produced a noticeable harmonic hum caused by blade runout and imbalance.

To reduce vibration and improve acoustic performance, the fan blades were manually trued using a dial indicator setup to measure blade offset and rotational consistency.

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/e036ffad-8aed-4081-8aab-e09118b92e57"
    alt="ThermaVault convection fan blade calibration"
    width="650">
</p>

<p align="center">
  <em>Dial indicator setup used to measure fan blade runout and correct blade alignment.</em>
</p>

### Calibration Process

- Mounted a dial indicator directly against the fan blade edge
- Rotated the fan assembly by hand to identify high and low spots
- Adjusted individual blade alignment incrementally
- Rechecked rotational consistency until runout was minimized

### Results

- Reduced harmonic vibration and fan resonance
- Lower audible hum during operation
  
Before Video-
https://github.com/user-attachments/assets/86a4d50e-11a0-4eb5-be31-e4b34c51b753



After Video-
https://github.com/user-attachments/assets/ccb41f80-d16f-4f0b-a22a-a5547bd761ed

---
