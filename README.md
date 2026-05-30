# Custom NFC Smart Card 

Hey! Welcome to the hardware repo for my custom NFC Smart Card. This project contains all the design files, manufacturing schematics, and assembly spreadsheets needed to get this board printed and assembled.

## What is this?
It's a 2-layer custom PCB smart card. Instead of buying a standard NFC tag, I designed this board to have the NFC antenna built right into the copper layers of the fiberglass itself. 

To make it interactive, it also rocks an onboard LED and a tactile switch.

## Hardware Specs
* **Thickness:** 1.6mm (Keeps it rigid so it doesn't snap in a wallet)
* **Color:** Blue Solder Mask
* **Finish:** LeadFree HASL
* **Parts Onboard:** NFC Chip, LED, Tactile Switch, Resistor, Capacitor

## The Files
Everything you need to manufacture this yourself is in this repo:
* **Gerber File:** The `.zip` file for printing the bare board.
* **BOM (Bill of Materials):** The `.csv` telling the factory what parts to buy.
* **CPL (Pick and Place):** The `.csv` telling the factory robots exactly where to solder those parts.

## How to Manufacture (JLCPCB Guide)
If you want to print this yourself, I highly recommend using JLCPCB. I've already formatted the files specifically for their assembly lines. Here is the cheat sheet for ordering:

1. Upload the Gerber `.zip`. 
2. Set the specs to **1.6mm** thickness, **Blue** color, and **LeadFree HASL**.
3. Turn on **PCB Assembly**. 
4. **Important:** Change the Assembly Type from Standard to **Economic PCBA** (Top Side only). This saves you like $30 in setup fees!
5. Upload the `BOM.csv` and `CPL.csv`. 
6. *Note:* When the system matches the parts, it will throw a red error for the `25X48MM_NFC_ANTENNA`. Just click **"Do Not Place"**. The antenna is already drawn into the copper, so the robots don't need to place a physical part for it.

Enjoy!
<br><br>
<img width="825" height="708" alt="image" src="https://github.com/user-attachments/assets/8f0234c9-d843-4525-9fd6-34094a417191" />
<img width="899" height="587" alt="Screenshot 2026-05-29 230642" src="https://github.com/user-attachments/assets/c15a5349-4ccb-479d-8750-e1b835baf60e" />
<img width="876" height="568" alt="Screenshot 2026-05-29 230636" src="https://github.com/user-attachments/assets/418f47ee-5e04-492c-849b-2eea199304f2" />

Note: ReadME was checked over by AI for grammar, sentence flow and structure!
