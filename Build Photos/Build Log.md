# ThermaVault PID — Build Log

## Overview

This document tracks the progression of the ThermaVault PID annealing oven conversion project.

The purpose of this build log is to document major design changes, thermal modifications, wiring improvements, and hardware integration throughout the development process.

The project is centered around converting a Breville convection oven into a more stable and serviceable PID-controlled process oven for annealing engineering plastics.

---

# Factory Control Panel Removal

The original Breville front control panel assembly was removed early in the build process to allow integration of a dedicated industrial PID controller and externalized control hardware.

The factory faceplate was retained temporarily during the CAD phase to establish dimensional references for the replacement panel design.

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

---

# Heater and Sensor Routing

Factory heater wiring was reorganized during the conversion process to improve serviceability and simplify future maintenance.

High-temperature insulated wire was retained within heated areas while routing paths were cleaned up and reorganized around the chamber.

Additional thermal protection sleeving and routing cleanup were implemented around heater pass-through locations and sensor entry points.

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
