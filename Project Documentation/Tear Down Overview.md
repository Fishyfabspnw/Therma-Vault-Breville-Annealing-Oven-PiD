# Breville BOV800XL Tear Down Documentation

## Oven Platform

Breville BOV800XL Smart Oven  
https://www.breville.com/en-us/product/bov800

This document covers the teardown and inspection process of the Breville BOV800XL convection oven platform used for the ThermaVault PID conversion project.

The teardown process is intended to:

- Understand the factory heater layout
- Identify factory thermal protection hardware
- Inspect airflow routing
- Document internal wiring layout
- Remove the factory control system
- Prepare the platform for PID conversion

<p align="center">
  <img width="300" height="225" alt="image" src="https://github.com/user-attachments/assets/388e833a-5e48-4bdd-87bd-afb590a3b30e" />
  <img width="300" height="225" alt="image" src="https://github.com/user-attachments/assets/ab8dee4d-45f8-4cd3-9a66-3d8479fedbdd" />
</p>

---

## Initial Disassembly

The outer shell is secured using multiple perimeter screws around the chassis.

Disassembly process:

1. Remove all visible perimeter screws.
2. Remove the hidden screws located underneath near the control board area.
3. Slide the shell rearward toward the back of the oven.
4. Lift the shell upward to fully remove the outer housing.

---

## Initial Observations

Once opened, several major factory systems become visible:

- Lower heater banks
- Factory convection fan
- Thermal protection devices
- Factory control PCB
- Internal airflow routing
- Heater wiring layout

<p align="center">
  <img width="720" alt="Internal oven layout" src="https://github.com/user-attachments/assets/a9642c1c-f821-4760-a027-971710ee7333" />
</p>

---

## Factory Heating System

The factory heating system consists of:

- Multiple upper heating elements
- Lower heating element banks
- Individually grouped heater circuits
- Convection-assisted airflow circulation

The heater groups appear to be separated into:

- Upper heater group(s)
- Lower heater group(s)

<p align="center">
  <img width="720" alt="Factory heater layout" src="https://github.com/user-attachments/assets/bd60366f-e9ca-4ef8-8a6a-9b2f9543b28a" />
</p>

---

## Factory Thermal Protection

The factory oven contains integrated thermal protection devices within the heater system wiring.

These devices are intended to:

- Interrupt power during overheating conditions
- Protect internal wiring and electronics
- Reduce fire risk
- Prevent unsafe chamber temperatures

The factory thermal protection system remains an important consideration during the ThermaVault PID conversion.

---

## Factory Parts Diagram Verification

The factory thermal fuse assembly was verified using the Breville BOV800XL parts diagram and component reference documentation.

The identified thermal protection assembly appears to match the factory-installed safety configuration used within the original heater circuit.

---

## Factory Thermal Fuse Reference

<p align="center">
  <img width="900" alt="Factory thermal fuse reference" src="https://github.com/user-attachments/assets/33cf837d-6fd7-42a2-909a-e1b01305b7c5" />
</p>
