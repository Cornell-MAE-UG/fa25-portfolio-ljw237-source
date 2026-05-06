---
layout: default
hidden: true
title: "ODP Milestone 4: Client Report"
permalink: /projects/odp/milestone4/
---

## Milestone 4 — Client Report

[← Back to ODP](/fa25-portfolio-ljw237-source/projects/odp/)

**Team:** Neil Morrison, Susanna Aufrichtig, Jamie Dalvito, Flavia Capet, and Luca Welle

---

### Context and Problem Statement

Spotted Lanternflies (SLFs) are an invasive species rapidly spreading across the eastern United States, posing a growing threat to agricultural systems. SLFs land on grape vines and feed on plant sugars, contaminating harvests, reducing yields, and worsening grape quality. They also excrete honeydew, promoting sooty mold that inhibits photosynthesis — costing the wine industry billions in lost yields. On-vine removal proved impractical due to the volume of insects and risk of vine damage, so our team explored attracting SLFs away from vines entirely.

---

### Final Prototype — VineGuard

![Final Prototype]({{ "/assets/images/odp_m4_prototype.png" | relative_url }})

![Labeled Prototype]({{ "/assets/images/odp_m4_labeled.png" | relative_url }})

VineGuard lures SLFs away from grapevines using a sugary attractant that mimics Tree of Heaven sap, then eliminates them using targeted vinegar spraying through servo-actuated side-mounted sprayers.

**1. Sap Attraction:** A sugar solution mimicking the viscosity of natural sap (~5 mPa·s) is pumped through a central pole, creating an attractive feeding source.

**2. Targeted Elimination:** Once insects gather, servo-actuated sprayers deliver vinegar to ethically dispose of them.

**Key Features:**
- Adjustable spray angles for coverage optimization
- Compact footprint for vineyard integration
- Arduino-controlled automation
- Low-toxicity vinegar-based treatment

A vineyard simply places the device, turns it on, and it runs autonomously with minimal maintenance.

---

### Assembly

![Assembly Process]({{ "/assets/images/odp_m4_assembly.png" | relative_url }})

![Assembly Detail]({{ "/assets/images/odp_m4_assembly_detail.png" | relative_url }})

![Servo Linkage]({{ "/assets/images/odp_m4_linkage.png" | relative_url }})

The box exterior can be rapidly assembled or disassembled. Each panel contains a lip to maintain box geometry, with screws attached throughout for rigidity. The lid consists of two pieces loosely press-fit to the top, giving quick access to interior electronics and fluid reservoirs for maintenance. Electrical components are wired using jumper wires and Wago connectors plugged directly into the Arduino. A 3D printed linkage allows servo motors to actuate the sprayer heads — a 3D printed bar screwed into the servo horn pulls the actuator forwards and backwards.

---

### Testing Details and Results

**Test 1 — Sap Drainage**

![Drainage Graph]({{ "/assets/images/odp_m4_graph_drainage.png" | relative_url }})

To test reservoir longevity, a mixture of 200g sucrose + 300g water (~5 mPa·s) was pumped for 10 minutes with water level recorded every 2.5 minutes.

**Result:** Drainage rate of 0.5 mL/min (6 mL/day) — a 1000 mL reservoir must be refilled every ~167 days.

---

**Test 2 — Spray Angle & Coverage**

![Coverage Graph]({{ "/assets/images/odp_m4_graph_coverage.png" | relative_url }})

Sprayers were tested at multiple angles to find maximum coverage of the central pole. The central pole was covered in paper, a spraying cycle was performed, and the damp area was measured.

**Result:** The optimal angle was **65 degrees**, achieving **86% spray coverage** — sufficient to cover the primary landing area of SLFs on the device.

---

**Test 3 — Battery Life**

| Component | Current Draw Active (mA) | Active Time (hr/day) | Daily Consumption (mAh/day) |
|---|---|---|---|
| Pump | 300 | 0.2 | 60 |
| Servo | 800 | 0.006 | 200.9 |
| Arduino | 40 | 24 | 960 |
| **Total** | | | **1220.9** |

| Parameter | Value |
|---|---|
| Battery Capacity | 10,000 mAh |
| Daily Usage | 1220.9 mAh |
| **Battery Life** | **~8.2 days** |

VineGuard can operate for approximately 8.2 days on a single 10,000 mAh charge. The modular battery design enables users to balance cost against serviceability depending on deployment needs.

---

### Bill of Materials

| Item | Vendor | Qty | Cost |
|---|---|---|---|
| Soft Masterkleer PVC Tubing (25ft) | McMaster Carr | 1 | $11.50 |
| Push to Connect Fitting | McMaster Carr | 6 | $15.66 |
| Kamoer NKP Peristaltic Pump | Amazon | 1 | $9.98 |
| M3 x 0.5 Socket Head Screw 14mm | McMaster Carr | 1 pack | $15.30 |
| 12V Power Supply | Taylor Design Studio | 1 | — |
| Metal Servo Arms Horn Aluminum | Amazon | 1 pack | $6.99 |
| Arduino Uno REV3 | Amazon | 1 | $27.60 |
| L298N Motor Driver | Amazon | 1 pack | $6.98 |
| LM2596 DC to DC Buck Converter | Amazon | 1 pack | $7.99 |
| Wago 221-415 Lever-Nuts | Amazon | 1 pack | $9.85 |
| Round Rocker Switches | Amazon | 1 pack | $6.39 |
| Spray Bottle 1 Gallon | McMaster Carr | 2 | $8.80 |
| Routing Clamp 15/16" ID | McMaster Carr | 2 | $7.42 |
| HDPE Plastic Bottle 1000mL | McMaster Carr | 2 | $7.46 |
| 2000 Series Dual Mode Servo | Taylor Design Studio | 1 | — |
| M3 x 0.5 Socket Head Screw 40mm | McMaster Carr | 1 pack | $4.86 |
| Zinc-Plated Steel Hex Nut M3 | McMaster Carr | 1 pack | $3.06 |
| **Total** | | | **$149.84** |

---

### Conclusion and Recommendation

VineGuard demonstrates strong potential as a feasible and effective solution for SLF protection. Testing confirmed the system can deliver attractant at controlled flow rates, achieve ideal spray coverage at 65 degrees, and operate for ~167 days autonomously on a full reservoir. The manufacturing and assembly process required minimal setup with low maintenance demands.

We recommend moving forward with field testing as the next step — specifically testing the attractant formulation, ideal vineyard placement, and aesthetic modifications to camouflage the device. VineGuard offers a low-toxicity, low-intervention, eco-friendly solution with the potential to save vineyards millions in yields compared to past pest control methods.

---

[← Previous: Milestone 3 — Functional Prototype](/fa25-portfolio-ljw237-source/projects/odp/milestone3/)