
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

## Fuse and Switch Clearance Modification

During test fitting, the original gray plastic structure behind the faceplate interfered with the added fuse holder and power switch. The extra plastic had to be removed so both components could sit fully into the panel without being forced or misaligned.

The first image shows the original gray plastic ribbing before modification. The second image shows the area after the plastic was broken out and cleared for the fuse and switch body.

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/5b16f992-9306-4360-84b6-7cb6bff306ad"
    alt="Gray plastic structure behind the faceplate before fuse and switch clearance modification"
    width="700">
</p>

<p align="center">
  <em>Original gray plastic behind the faceplate that interfered with the fuse holder and switch fitment.</em>
</p>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/2f87ea5d-049a-4637-95e4-d316b0342d5f"
    alt="Gray plastic removed from behind the faceplate to allow fuse holder and switch clearance"
    width="700">
</p>

<p align="center">
  <em>Plastic cleared from the rear of the faceplate so the fuse holder and power switch could seat properly.</em>
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

## Shell Reassembly and Control Box Fitment

After the wiring inspection was complete, the outer shell was reinstalled around the oven body. During reassembly, the mounting locations were checked carefully so the shell could be seated without pinching wires or forcing the panels out of alignment.

The rear control box also required extra reach to reinstall the screws cleanly. A drill extension was used to access the recessed fasteners and tighten the control box back into place after the shell was fitted.

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/8a16767d-b571-48c7-8b2a-4a25632db435"
    alt="Pointing to oven shell mounting location during reassembly"
    width="700">
</p>

<p align="center">
  <em>Checking shell mounting locations before reinstalling the outer cover.</em>
</p>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/7d64c555-e9fc-474a-b308-1eb606125480"
    alt="Second shell mounting location reference during oven reassembly"
    width="700">
</p>

<p align="center">
  <em>Additional mounting point reference used while lining up the oven shell.</em>
</p>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/0d156078-f6c1-41a2-90f6-e9b8609dc725"
    alt="Drill extension needed to reach recessed control box screws"
    width="700">
</p>

<p align="center">
  <em>Drill extension used to reach the recessed screws for the rear control box.</em>
</p>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/e7cdaa90-e199-4ef2-8552-b962c3a8c3b9"
    alt="Using drill extensions to reinstall the oven control box screws"
    width="700">
</p>

<p align="center">
  <em>Reinstalling the control box screws with extensions after the shell was positioned.</em>
</p>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/ca8f5fa6-109c-4cab-bc1c-b958e790be44"
    alt="Oven shell reinstalled and ThermaVault PID powered on"
    width="700">
</p>

<p align="center">
  <em>Shell reinstalled and the oven powered on for the next stage of testing.</em>
</p>

### Reassembly Notes

- Verified shell mounting points before tightening screws
- Checked that the shell did not pinch or pull on wiring
- Used drill extensions to reach recessed control box fasteners
- Confirmed the rear electronics area remained serviceable after reassembly
- Powered the oven on after the shell was reinstalled for the next round of functional testing

---

## Controller Setup, First PID Tune, and First Annealing Cycle

With the oven reassembled and powered on, the next stage was setting up the PID controller through the phone app and preparing the oven for its first controlled heat cycle.

The controller was connected through the app so the process temperature, setpoint, output behavior, and tuning status could be monitored without relying only on the front panel display. This made it easier to watch the oven during early testing and confirm that the controller was responding correctly.

### Initial Controller Setup

The first setup pass focused on confirming the basics before running a full annealing cycle:

- Verified that the PT100 temperature reading was stable and believable at room temperature
- Confirmed the controller was in automatic control mode, not manual output mode
- Checked that the SSR output switched the heating elements on and off correctly
- Verified that the convection fan operated as expected
- Set a conservative test temperature before moving into higher-temperature annealing profiles
- Watched the app display to confirm that the process value followed the setpoint correctly

This step was important because manual output mode can drive the heating elements continuously. For normal annealing use, the controller needs to regulate temperature automatically through the SSR.

### First PID Autotune

After basic operation was confirmed, the first PID autotune was started with the oven empty and under direct supervision. The goal of the autotune was to let the controller learn how the modified oven responds to heat input, insulation, convection airflow, and thermal lag.

During tuning, the controller cycles the heater output and watches how the chamber temperature rises, overshoots, falls, and stabilizes. From that response, it calculates new PID values for proportional, integral, and derivative control.

The first tune is not treated as the final tune forever. It is a baseline tune for the current oven configuration. Any major change to insulation, sensor placement, heater wiring, fan behavior, or chamber load may require tuning again.

### First Annealing Test

Once the controller completed its first tune, the oven was used for an initial annealing test. This first run was treated as a validation cycle rather than a production cycle.

The purpose of the first annealing run was to confirm:

- The oven could reach the target temperature without uncontrolled overshoot
- The controller could hold a stable temperature after heat soak
- The SSR and heat sink remained stable during repeated heater cycling
- The convection fan continued to move air through the chamber
- The wiring and shell remained mechanically stable after heating
- The chamber cooled down normally after the cycle

For the first real material test, the oven should be watched closely from heat-up through cooldown. The goal is not just to make the plastic hot. The goal is to prove that the converted oven behaves predictably enough to become a repeatable annealing tool.

### First-Cycle Notes

- Run the first cycle empty or with a low-risk test part before trusting critical parts
- Stay with the oven during the first full heat cycle
- Watch for smell, smoke, wire movement, abnormal fan noise, or unstable temperature behavior
- Confirm the SSR heat sink temperature stays reasonable during cycling
- Let the oven cool down naturally before opening it aggressively or removing parts
- Record the first usable temperature profile so future cycles can be compared against it

> **Build note:** The first PID tune and first annealing cycle are part of commissioning the oven. They should be treated as controlled testing, not normal unattended operation.

---