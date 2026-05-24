# ThermaVault PID

**Industrial-style PID-controlled annealing oven conversion based on a Breville convection oven platform.**

ThermaVault PID is a documentation-first appliance conversion project focused on creating a more stable, serviceable, and repeatable annealing oven for engineering plastics used in 3D printing.

The build replaces the factory appliance timer/control behavior with an industrial PID controller, solid state relay heater control, high-temperature sensing, upgraded insulation, and a more modular electronics layout.

> **Status:** Active build / documentation in progress  
> **Platform:** Breville convection oven conversion  
> **Use case:** Controlled annealing cycles for 3D printed engineering plastics

<p align="center">
  <img width="720" alt="ThermaVault oven build" src="https://github.com/user-attachments/assets/534b35a8-9bc2-4163-81de-b93c42fc987d" />
</p>

---

## Table of Contents

- [Project Goals](#project-goals)
- [System Overview](#system-overview)
- [Core Hardware](#core-hardware)
- [Documentation](#documentation)
- [Bill of Materials](#bill-of-materials)
- [Photos](#photos)
- [Safety Notice](#safety-notice)
- [License](#license)

---

## Project Goals

ThermaVault is being built as a compact process oven platform with a focus on:

- Stable annealing temperatures
- Reduced thermal overshoot
- Better chamber temperature consistency
- Programmable ramp/soak heat cycles
- Serviceable wiring and component layout
- Industrial-style process control hardware
- Improved insulation for long-duration heat stability
- Reusable appliance platform for future refinement

This is not meant to be a quick “add a PID and call it good” project. The goal is to build a cleaner, safer, better-documented oven conversion that can be maintained, upgraded, and understood later.

---

## System Overview

At a high level, the oven uses a PID controller to read chamber temperature and control the heating elements through a properly rated AC solid state relay.

```text
AC Power In
   |
   |-- Fuse / breaker protection
   |-- Main power switch
   |-- PID controller power
   |-- Convection fan control
   |
   '-- SSR-controlled heater circuit
          |
          '-- Factory heating elements
```

The factory convection fan is retained so the oven can continue circulating hot air through the chamber. Temperature feedback is handled by a high-temperature sensor mounted for chamber/process temperature control.

<p align="center">
  <img width="420" alt="PID controller" src="https://github.com/user-attachments/assets/1f51fc1a-f9c9-4be2-b712-107a3e9f7998" />
  <img width="380" alt="SSR hardware" src="https://github.com/user-attachments/assets/84f70611-4241-4cf7-9cf8b605c220" />
</p>

---

## Core Hardware

| System | Component | Notes |
|---|---|---|
| Oven platform | Breville convection oven | Donor appliance chassis and heating chamber |
| Temperature control | Novus N20K48 PID controller | Main process controller with ramp/soak capability |
| Heater switching | Industrial zero-cross AC SSR | SSR must be properly rated and mounted to a heat sink |
| Temperature sensing | RTD PT100 | Chamber/process temperature feedback |
| Airflow | Factory convection fan | Retained for chamber circulation |
| Protection | Fuse / breaker / thermal cutoff | Required safety hardware, not optional |
| Wiring | High-temperature appliance wire | Use properly rated wire for hot zones |
| Insulation | Ceramic fiber insulation | Used to improve chamber stability |

---

## Documentation

| Document | Purpose |
|---|---|
| [Bill of Materials](./BOM.md) | Current parts list, links, quantities, and notes |
| [Safety Notes](./SAFETY.md) | Mains voltage, heat, SSR, fuse, and enclosure safety notes |
| [Wiring Overview](./docs/WIRING_OVERVIEW.md) | High-level wiring architecture and circuit notes |
| [Build Notes](./docs/BUILD_NOTES.md) | Build planning, layout notes, and documentation checklist |
| [Tear Down Photo Log](./Build%20Photos/Tear%20Down%20Overview.md) | Photo documentation from the oven teardown |

---

## Bill of Materials

The BOM has been moved to a dedicated file so it can grow without cluttering the main README.

See: **[BOM.md](./BOM.md)**

---

## Photos

Current photo documentation:

- [Tear Down Photo Log](./Build%20Photos/Tear%20Down%20Overview.md)

Future photo sections to add:

- Original oven overview
- Factory wiring before modification
- Controller layout
- SSR and heat sink mounting
- Sensor placement
- Final faceplate / enclosure install
- First heat test

---

## Safety Notice

> **Warning:** This project involves mains AC voltage, high temperatures, resistive heating elements, appliance modification, and long-duration unattended heat risk. Mistakes can cause electric shock, fire, equipment damage, or injury.

Minimum safety expectations:

- Use properly rated fuses or breakers.
- Maintain chassis ground continuity.
- Use high-temperature wire inside hot zones.
- Mount the SSR to a correctly sized heat sink.
- Keep low-voltage and mains-voltage wiring separated.
- Use strain relief on incoming power.
- Do not bypass factory thermal safety devices unless they are replaced with equal or better protection.
- Verify wiring with a meter before applying power.
- Perform initial heat tests attended and away from flammable material.

Read the full safety page before copying any part of this build: **[SAFETY.md](./SAFETY.md)**

---

## Project Direction

Planned documentation improvements:

- Wiring diagram
- Faceplate CAD files
- Controller parameter notes
- Annealing cycle examples
- Thermal test results
- Chamber temperature stability data
- Final assembly photos

---

## License

This project is licensed under the **GNU GPL v3.0 License**.

---

## FishyFabsPNW

Designed, built, and documented by **FishyFabsPNW**.
