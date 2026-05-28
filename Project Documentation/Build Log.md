
# ThermaVault PID — Build Log

## Overview

This document tracks the progression of the ThermaVault PID annealing oven conversion project.

The purpose of this build log is to document major design changes, thermal modifications, wiring improvements, and hardware integration throughout the development process.

The project is centered around converting a Breville convection oven into a more stable and serviceable PID-controlled process oven for annealing engineering plastics.

---

# Factory Control Panel Removal and Faceplate Development

The original Breville front control panel assembly was removed early in the build process to allow integration of a dedicated industrial PID controller and externalized control hardware.

The factory faceplate was retained during the tear down phase so it could be repurposed into a new control layout instead of starting from a completely blank panel.

<p align="center">
  <img width="420" alt="Factory control panel" src="https://github.com/user-attachments/assets/0ee69a7e-09fd-4fe2-8b7a-6b8b25b1fa56" />
</p>

<p align="center">
  <em>Original Breville control panel removed during tear down for conversion into the new ThermaVault PID control interface.</em>
</p>

A custom replacement faceplate was then designed and fabricated to integrate the industrial PID controller and external power controls into a cleaner and more serviceable layout.

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

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/d88b5516-448a-4d09-acd3-1fd51a605652"
    alt="Kwool ceramic insulation added around the oven shell"
    width="700">
</p>

<p align="center">
  <em>Kwool ceramic insulation added around the oven shell to improve heat retention and reduce heat loss through the outer body.</em>
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

## Convection Fan Calibration

During initial testing, the factory convection fan assembly produced a noticeable harmonic hum. The fan was still functional, but the blade assembly had enough runout and imbalance to create vibration and resonance during operation.

To correct this, the fan blades were manually trued using a dial indicator. Each blade was checked by rotating the fan by hand, identifying high and low spots, and carefully adjusting the blade position until the runout was reduced.

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/e036ffad-8aed-4081-8aab-e09118b92e57"
    alt="ThermaVault convection fan blade calibration"
    width="650">
</p>

<p align="center">
  <em>Dial indicator setup used to measure fan blade runout and correct blade alignment before final fan testing.</em>
</p>

### Calibration Steps

- Mounted a dial indicator against the outer edge of the fan blades
- Rotated the fan assembly by hand to check blade-to-blade consistency
- Identified high and low spots in the blade path
- Adjusted individual blades in small increments
- Rechecked the fan until the runout and visible wobble were reduced

### Before Calibration

Before adjustment, the fan had visible runout and produced a stronger harmonic hum during operation. This made the fan sound rougher than expected and showed that the blade assembly was not spinning evenly.

https://github.com/user-attachments/assets/86a4d50e-11a0-4eb5-be31-e4b34c51b753

### After Calibration

After truing the blades, the fan ran noticeably smoother with less vibration and a lower audible hum. This should help reduce resonance in the oven shell during long annealing cycles.

https://github.com/user-attachments/assets/ccb41f80-d16f-4f0b-a22a-a5547bd761ed

### Result

- Reduced fan vibration
- Lower harmonic hum during operation
- Smoother convection fan rotation
- Less resonance transferring into the oven shell

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

## SSR Installation and Heat Sink Mounting

The solid state relay was mounted to an aluminum heat sink using thermal paste between the SSR and the heat sink surface. The thermal paste improves heat transfer from the SSR into the heat sink during heater cycling.

After the SSR was attached to the heat sink, the heat sink assembly was bolted to the metal shell of the oven. This gives the SSR a solid mechanical mounting point and allows the oven shell to act as additional thermal mass.

This location keeps the SSR close to the heater wiring path while still keeping it mounted outside the primary heated chamber area.

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/e6866fe5-152b-4cad-b7b4-a251963c89cc"
    alt="SSR mounted to heat sink and bolted to the oven shell"
    width="700">
</p>

<p align="center">
  <em>SSR mounted with thermal paste to a heat sink, then bolted to the oven shell for improved heat dissipation and serviceable wiring layout.</em>
</p>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/0986bab6-bab5-4aef-b042-77a3bac9bf72"
    alt="Additional view of SSR heat sink mounting and rear wiring layout"
    width="700">
</p>

<p align="center">
  <em>Additional rear view showing the SSR heat sink location, nearby WAGO distribution blocks, and wiring path around the heater control area.</em>
</p>

> **Build note:** The SSR should be mounted tightly against the heat sink with thermal paste applied between the two surfaces. Wiring should be kept clear of the heat sink body and high-voltage terminals.

---

## Wiring Inspection Before Shell Reassembly

Before reinstalling the outer shell, the wiring layout was checked over with the oven still open. This is the best time to verify that all high-voltage connections are seated, all terminals are tight, and nothing can rub against sharp sheet-metal edges once the cover is installed.

This inspection step is especially important because once the shell is back on, access to the SSR, WAGO distribution blocks, sensor routing, and heater wiring becomes much more limited.

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/614671fd-78d4-4925-8707-2505f6e3b56f"
    alt="Open rear wiring inspection before reinstalling the oven shell"
    width="700">
</p>

<p align="center">
  <em>Final open-shell wiring check before reinstalling the oven cover.</em>
</p>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/9e315309-9e3b-4f30-9069-b5df3ce45882"
    alt="Additional wiring inspection view before reinstalling the oven shell"
    width="700">
</p>

<p align="center">
  <em>Additional inspection angle showing the rear wiring, terminal layout, and clearance checks before the shell was reinstalled.</em>
</p>

### Pre-Reassembly Checks

- Confirm all WAGO levers are fully closed
- Verify all screw terminals are tight
- Check that high-temperature wire is used anywhere exposed to heat
- Keep mains-voltage wiring separated from sensor and control wiring where possible
- Make sure wires cannot contact heater elements, sharp sheet metal, or the convection fan
- Confirm the SSR and heat sink are securely mounted
- Verify chassis ground continuity before powering the oven again

> **Safety note:** Do not reinstall the shell until the wiring has been visually inspected and verified with a meter where needed. This build uses mains AC voltage, so any loose connection or misplaced wire can become a serious shock or fire hazard.

---