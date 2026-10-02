# ThermaVault Community Builds

This directory is for builds that use the **ThermaVault PID project as a starting point** but adapt it to a different oven model, enclosure, control-panel layout, or hardware arrangement.

Keeping each adaptation in its own folder makes it possible to add more models without turning the main project README into one long photo log.

---

## Build Index

| Oven / Platform | Build page | Model-specific files |
|---|---|---|
| **Breville BOV650** | [View BOV650 build](./BOV650/README.md) | [FacePlate_BOV650.step](../../CAD%20Models/FacePlate_BOV650.step) |

---

## Folder Layout

Each community build should use its own model folder:

```text
Project Documentation/
└── Community Builds/
    ├── README.md
    ├── BUILD_TEMPLATE.md
    ├── BOV650/
    │   ├── README.md
    │   ├── bov650-community-build-front.jpg
    │   ├── bov650-community-build-controls.jpg
    │   └── bov650-community-build-angle.jpg
    └── <NEXT_MODEL>/
        ├── README.md
        └── photos...
```

Model-specific CAD can stay in the main **[CAD Models](../../CAD%20Models/)** directory so printable/CAD files remain easy to find from one place.

---

## Adding Another Build

1. Copy **[BUILD_TEMPLATE.md](./BUILD_TEMPLATE.md)** into a new folder named after the oven model.
2. Rename it to `README.md`.
3. Add the build photos to that same folder.
4. Add any model-specific CAD to the main `CAD Models/` directory.
5. Add the new model to the **Build Index** table above.
6. Add a short link under **Community Builds** in the root project README if you want it featured there.

---

## Important

Community adaptations may use different dimensions, wiring layouts, heating elements, controls, thermal protection, or factory hardware than the original ThermaVault build. Treat each build as a reference for that specific platform and verify dimensions, electrical ratings, grounding, fusing, and thermal safety before applying it to another oven.
