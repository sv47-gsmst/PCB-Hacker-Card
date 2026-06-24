# Custom NFC Smart Card

My custom NFC smart card project. Has all the files to build and order the PCB.

## Features
* **Built-in Antenna:** Etched right into the PCB copper. No external wire needed.
* **No Code:** Uses an NT3H2111W0FHKH chip. Runs on wireless power with zero code.
* **Button & LED:** Includes a clicky switch and an LED to test it.

---

## Files
* `BOM_Hack-Card_2026-05-29.csv` – Parts list and links.
* `Gerber_Hack-Card_PCB_Hack-Card_2026-05-29...zip` – PCB layout files.
* `PickAndPlace_PCB_Hack-Card_2026-05-29.csv` – Component coordinates for assembly.
* `Hack Card_5c9b41320e854d2689e4a3fa391419...zip` – EasyEDA project file.
* `3D_1-PCB_PCB_Hack Card_2026-06-15.step` – 3D model.

---

## Specs
* **Thickness:** 1.6mm (won't snap in a wallet)
* **Color:** Blue Gloss
* **Layers:** 2 layers
* **Finish:** Lead-Free HASL

---

## How to Order (JLCPCB)
1. Upload `Gerber...zip`.
2. Choose **1.6mm thickness**, **Blue solder mask**, and **Lead-Free HASL**.
3. Turn on **PCB Assembly** and pick **Economic (Top Side Only)**.
4. Upload `BOM...csv` and `PickAndPlace...csv`.
5. **CRITICAL:** The preview will show an error for `25X48MM_NFC_ANTENNA`. Set it to **Do Not Place (DNP)**. The antenna is just copper traces, there is no physical part.

---

## Parts
* **NFC Chip:** [NT3H2111W0FHKH (C710403)](https://jlcpcb.com/partdetail/NxpSemicon-NT3H2111W0FHKH/C710403)
* **Button:** [TS-1187A-B-A-B (C318884)](https://jlcpcb.com/partdetail/XkbConnectivity-TS_1187A_B_AB/C318884)
* **Resistor:** [47Ω 0603 (C23182)](https://jlcpcb.com/partdetail/23909-0603WAF470JT5E/C23182)
* **LED:** [Green-Yellow 0805 (C2296)](https://jlcpcb.com/partdetail/EverlightElec-1721SUYCTR8/C2296)
* **Capacitor:** [220nF 0603 (C21120)](https://jlcpcb.com/partdetail/SamsungElectroMechanics-CL10B224KA8NNNC/C21120)
<br><br>
<img width="825" height="708" alt="image" src="https://github.com/user-attachments/assets/8f0234c9-d843-4525-9fd6-34094a417191" />
<img width="899" height="587" alt="Screenshot 2026-05-29 230642" src="https://github.com/user-attachments/assets/c15a5349-4ccb-479d-8750-e1b835baf60e" />
<img width="876" height="568" alt="Screenshot 2026-05-29 230636" src="https://github.com/user-attachments/assets/418f47ee-5e04-492c-849b-2eea199304f2" />

Note: ReadME was checked over by AI for grammar, sentence flow and structure!
