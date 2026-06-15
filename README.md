# Custom NFC Smart Card 💳⚡

Welcome to the hardware development repository for my custom NFC Smart Card. This project contains the comprehensive engineering documentation, automated manufacturing assets, interactive circuit logic, and source design environments required to fabricate, populate, and deploy this custom hardware device.

## ✨ Core System Features
* **Integrated Planar NFC Antenna:** A multi-turn inductive micro-strip coil etched natively across the primary copper layout layers, eliminating the need for an external wire-wound component.
* **Passive RF Communication Node:** Powered entirely over-the-air via the integrated `NT3H2111W0FHKH` NTAG I2C IC. The passive chip functions without local system firmware execution, requiring no text-based source code compilation steps.
* **Onboard Interactive Controls:** Includes a dedicated tactile micro-switch circuit routing to a status indicator LED array for physical validation testing.

---

## 📁 Repository Structure & Inventory
This repository contains the absolute minimum file-set required for complete end-to-end industrial reproduction:

* **`BOM_Hack-Card_2026-05-29.csv`** – The structured Bill of Materials detailing physical device specifications, part classifications, and direct vendor acquisition links.
* **`Gerber_Hack-Card_PCB_Hack-Card_2026-05-29...zip`** – Complete manufacturing photoplotter artwork data specifying structural routing, drill files, traces, and mask geometries.
* **`PickAndPlace_PCB_Hack-Card_2026-05-29.csv`** – Structured component placement data mapping specific coordinate metrics, rotation profiles, and trace centerlines for pick-and-place manufacturing robotics.
* **`Hack Card_5c9b41320e854d2689e4a3fa391419...zip`** – The master source project archive. This contains the native, uncompiled schematic diagrams and layout geometry files readable by the EasyEDA CAD ecosystem.
* **`3D_1-PCB_PCB_Hack Card_2026-06-15.step`** – Comprehensive solid-body geometric 3D CAD definition file for integration into structural mechanical software like Fusion 360, SolidWorks, or FreeCAD.

---

## 🛠️ Bare-Board Structural Specifications
* **Substrate Material Thickness:** 1.6mm (Standard rigid composition selected to prevent trace fracturing or component delamination inside regular wallets).
* **Primary Solder Mask Profile:** Blue Gloss
* **Layer Composition Strategy:** 2-Layer Layout (Top/Bottom)
* **Surface Topography Finish:** Lead-Free HASL (RoHS compliant formulation optimized for automated surface assembly lines).

---

## 🏭 Automated SMT Assembly Instructions (JLCPCB)
This hardware project is pre-formatted for direct compatibility with JLCPCB’s automated SMT manufacturing lines. When ordering, execute the following parameters:

1. Upload the structural `Gerber...zip` archive directly to the online quoting parsing engine.
2. Verify hardware characteristics are matched to: **1.6mm thickness**, **Blue solder mask**, and **Lead-Free HASL**.
3. Enable the **PCB Assembly** toggle option and select **Economic PCBA (Top Side Only)** to bypass unnecessary multi-side tooling costs.
4. Upload the accompanying component alignment and inventory files when prompted: `BOM...csv` and `PickAndPlace...csv`.
5. ⚠️ **Critical Production Note:** The automated footprint alignment inspector will flag the component identifier `25X48MM_NFC_ANTENNA` as an unmatched part error. Instruct the manufacturer to tag this specific line item as **"Do Not Place" (DNP)**. The antenna system is integrated directly into the printed copper tracking of the board itself, requiring zero physical part assembly.

---

## 🔗 Component Sourcing Directory
Direct manufacturer links matching the exact JLCPCB part codes utilized on this card assembly:

* **Passive NFC Chip (U1):** [NT3H2111W0FHKH (JLCPCB Part # C710403)](https://jlcpcb.com/partdetail/NxpSemicon-NT3H2111W0FHKH/C710403)
* **Tactile Micro-Switch (SW1):** [TS-1187A-B-A-B (JLCPCB Part # C318884)](https://jlcpcb.com/partdetail/XkbConnectivity-TS_1187A_B_AB/C318884)
* **SMD Fixed Resistor (R1):** [47Ω 0603 Resistor (JLCPCB Part # C23182)](https://jlcpcb.com/partdetail/23909-0603WAF470JT5E/C23182)
* **SMD Emitting Diode (LED1):** [Yellow-Green LED 0805 (JLCPCB Part # C2296)](https://jlcpcb.com/partdetail/EverlightElec-1721SUYCTR8/C2296)
* **SMD Ceramic Capacitor (C1):** [220nF 0603 Capacitor (JLCPCB Part # C21120)](https://jlcpcb.com/partdetail/SamsungElectroMechanics-CL10B224KA8NNNC/C21120)
<br><br>
<img width="825" height="708" alt="image" src="https://github.com/user-attachments/assets/8f0234c9-d843-4525-9fd6-34094a417191" />
<img width="899" height="587" alt="Screenshot 2026-05-29 230642" src="https://github.com/user-attachments/assets/c15a5349-4ccb-479d-8750-e1b835baf60e" />
<img width="876" height="568" alt="Screenshot 2026-05-29 230636" src="https://github.com/user-attachments/assets/418f47ee-5e04-492c-849b-2eea199304f2" />

Note: ReadME was checked over by AI for grammar, sentence flow and structure!
