---
layout: default
hidden: true
title: "ODP Milestone 3: Functional Prototype"
permalink: /projects/odp/milestone3/
---

## Milestone 3 — Functional Prototype

[← Back to ODP](/fa25-portfolio-ljw237-source/projects/odp/)

**Team:** Save the Grapes — Neil, Susanna, Jamie, Flavia, and Luca

---

### Overview

![CAD Render]({{ "/assets/images/odp_m3_cad.png" | relative_url }})

The functional prototype is a single-column device consisting of a wooden box base with a PVC pipe extending vertically, wrapped in tubing that slowly drips Tree of Heaven sap to attract spotted lanternflies. A 3D printed shower head at the top disperses vinegar to ethically dispose of attracted insects.

---

### Design Intent

![Design Sketch]({{ "/assets/images/odp_m3_cad_sketch.png" | relative_url }})

The prototype consists of three main systems:
- **Structure** — A balsa wood box base with a 3D printed door and PVC pipe column
- **Fluid System** — Two tubes running through the PVC pipe: one wrapped externally to drip sap, one internal delivering vinegar to the shower head
- **Shower Head** — A 3D printed dome with channels that disperses vinegar in a radius around the device

![Labeled CAD]({{ "/assets/images/odp_m3_cad_labeled.png" | relative_url }})

![CAD Views]({{ "/assets/images/odp_m3_cad_open.png" | relative_url }})

---

### Bill of Materials

| Item | Vendor | Quantity | Cost |
|---|---|---|---|
| Soft Masterkleer PVC Tubing (5mm) | McMaster Carr | 25 ft | $11.50 |
| Surface-Mount Hinge with Holes | McMaster Carr | 4 | $5.32 |
| Push to Connect Fitting | McMaster Carr | 6 | $15.66 |
| White Plastic Corner Bracket | McMaster Carr | 20 | $2.60 |
| Kamoer NKP Low Flow Peristaltic Pump | Amazon | 1 | $9.98 |
| M3 x 0.5 Socket Head Screw 14mm | McMaster Carr | 1 pack | $15.30 |
| Zinc-Plated Steel Hex Nut M3 | McMaster Carr | 1 pack | $3.06 |
| 0.25in Wood Panels (4in x 10in) | Taylor Design Studio | 4 | — |
| 0.25in Wood Panels (4in x 8in) | Taylor Design Studio | 1 | — |
| 3D Printed Parts (brackets, door, sprayer head) | RPL | various | — |
| 12V Power Supply | Taylor Design Studio | 1 | — |
| **Total** | | | **$63.42** |

---

### Assembly Process

**Box Base**
Cut four balsa planks to 10in and one to 8in. Assemble into a box without a front or bottom using corner brackets and screws. Attach the 3D printed door frame with corner attachments and use hinges to mount the door. Cut a hole through the middle of the top using a hole saw for the PVC pipe.

**PVC Pipe & Tubing**
- Inner tubing (vinegar): 43in — runs through the center of the PVC pipe to the shower head
- Wrapped tubing (sap): 96in — exits at 4.5in from bottom, wraps around the pipe, re-enters at the top
- Make small Xacto knife incisions every 1/16in along the wrapped tubing for sap to drip out
- PVC pipe length: 36in

---

### Design Testing

![Test 1 — Incision Flow]({{ "/assets/images/odp_m3_test1.png" | relative_url }})

**Test 1 — Incision Flow Rate**

Water was used as a test fluid. Small Xacto knife incisions were made in the wrapped tubing and flow was measured over 10 minutes.

| Time (min) | Solution in bottle (mL) |
|---|---|
| 0 | 400 |
| 2.5 | 399 |
| 5 | 398 |
| 7.5 | 397 |
| 10 | 395 |
| **Avg flow rate** | **0.5 mL/min** |

The average flow rate of 0.5 mL/min confirmed our assumption that incision flow would be very small — suitable for lasting several days before refilling.

![Test 2 — Shower Head Flow]({{ "/assets/images/odp_m3_test2.png" | relative_url }})

**Test 2 — Shower Head Flow Rate**

| Time (min) | Solution (mL) |
|---|---|
| 0 | 370 |
| 0.5 | 320 |
| 1 | 300 |
| 1.5 | 250 |
| 2 | 200 |
| 2.5 | 150 |
| 3 | 100 |
| **Flow rate** | **90 mL/min** |

The shower head flow rate was 30x higher than the incision design due to the larger cross-sectional area — matching our expectations.

---

### Success Criteria

**(1) Sap Drainage Rate < 20 mL/hr**
Current drainage is ~180 mL/hr — needs to be reduced. Options include lowering drive voltage or adding a clamp to limit flow. At 20 mL/hr, a 500mL reservoir would last approximately one day (scaled to once per week in the real-world model).

**(2) Vinegar Sprayer Radius > 0.25m**
Not yet measured. Will be tested by running the shower system for 30 seconds over paper and measuring the farthest droplet. Shower head can be redesigned to curve inward like an umbrella to direct spray toward the pipe.

**(3) Electronics & Fluid Storage within 320 cubic inches**
Both reservoirs and electronics must fit within the box base. Fluid storage should be maximized while protecting electronics.

---

[← Previous: Milestone 2 — First Prototype](/fa25-portfolio-ljw237-source/projects/odp/milestone2/)
[Next: Milestone 4 — Client Report →](/fa25-portfolio-ljw237-source/projects/odp/milestone4/)