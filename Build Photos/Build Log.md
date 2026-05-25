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

# Heater and Sensor Routing

Factory heater wiring was reorganized during the conversion process to improve serviceability and simplify future maintenance.

High-temperature insulated wire was retained within heated areas while routing paths were cleaned up and reorganized around the chamber.

Additional thermal protection sleeving and routing cleanup were implemented around heater pass-through locations and sensor entry points.

<p align="center">
  <img width="420" alt="Sensor routing closeup" src="https://github.com/user-attachments/assets/cac5710c-9792-4d3d-9450-c5601a9212b5" />
</p>

<p align="center">
<i>High-temperature sleeving and routing cleanup around chamber wire pass-through locations.</i>
</p>

<p align="center">
<i>Close-up view of insulated chamber wiring and thermal protection routing.</i>
</p>

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

# Convection Fan Retention

The factory convection fan system was retained as part of the chamber airflow strategy.

Maintaining airflow circulation helps improve chamber temperature uniformity and reduces localized hot spots during long-duration annealing cycles.

The fan assembly and surrounding wiring were reorganized during the conversion process to integrate with the updated wiring architecture.

---

# Custom Faceplate Development

A custom replacement faceplate was designed and fabricated to integrate the industrial PID controller and external power controls.

The replacement panel relocates process controls outside the primary heated cavity while creating a cleaner and more purpose-built interface compared to the original appliance controls.

The faceplate was CAD-modeled specifically around the oven chassis geometry and mounting constraints.

Current control system features include:

- Industrial PID controller integration
- Externalized power switching
- Improved serviceability
- Reduced exposure to chamber heat

The control panel remains actively under development as the project continues to evolve.

---

# Current Build State

At the current stage of development, the oven has transitioned from a factory countertop appliance into a dedicated PID-controlled process oven platform featuring:

- Improved chamber sealing
- Additional thermal insulation
- Modular DIN rail wiring distribution
- Industrial-style process controls
- Externalized control hardware
- Improved serviceability and maintenance access

The project remains under active development as additional testing and refinement continue.
