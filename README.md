# 30A Home Automation using ESP32 – PCB Design with KiCad

##  Project Overview
This project focuses on the design and development of a custom PCB for a 30A-rated home automation system using the ESP32 microcontroller. The aim is to control high-current appliances remotely via Wi-Fi, while ensuring safety, compact design, and low cost.
![3D View](WhatsApp%20Image%202025-06-17%20at%2014.47.17_306fb640.jpg)


---

##  Tools Used
- **KiCad**: For schematic capture, PCB layout, and 3D visualization.
- **ESP32 Dev Module**: As the main controller.
- **Relay Module / SSR (30A rated)**: For switching high-power devices.
- **Other Components**: Resistors, diodes, optocoupler (for isolation), connectors, capacitors, voltage regulators (like AMS1117), screw terminals.

---

##  Design Process Using KiCad

### 1. **Creating the Schematic**
- Launched KiCad and started a new project.
- Added components like ESP32, relays, flyback diodes, optocouplers, and screw terminals.
- Wired the components logically ensuring proper power rails and ground.
- Assigned appropriate component values.
- Verified electrical rules (ERC).

  
## Component Footprints (KiCad)

| Ref     | Component             | Footprint                                               |
|---------|-----------------------|----------------------------------------------------------|
| C1      | 10uF Capacitor        | Capacitor_SMD:C_0805_2012Metric                          |
| C2      | 22uF Capacitor        | Capacitor_SMD:C_0805_2012Metric                          |
| D1      | 1N4148 Diode          | Diode_THT:D_DO-35_SOD27_P7.62mm_Horizontal               |
| D2      | 1N4148 Diode          | Diode_THT:D_DO-35_SOD27_P7.62mm_Horizontal               |
| D3      | LED                   | LED_SMD:LED_0805_2012Metric                              |
| D4      | LED                   | LED_SMD:LED_0805_2012Metric                              |
| H1–H4   | Mounting Holes        | MountingHole:MountingHole_2.7mm_M2.5_Pad_Via             |
| J1      | 4-pin Connector       | Connector_PinHeader_2.54mm:PinHeader_1x04_P2.54mm_Vertical |
| J2      | 4-pin Terminal Block  | TerminalBlock:TerminalBlock_bornier-4_p5.08mm            |
| J3      | 3-pin Terminal Block  | TerminalBlock:TerminalBlock_bornier-3_p5.08mm            |
| K1      | Relay (RAYEX-L90AS)   | Relay_THT:Relay_SPST_RAYEX-L90AS                         |
| K2      | Relay (PR13-5V-450)   | RELAY_PR13-5V-450-1C                                     |
| PS1     | HLK-PM01 Converter    | Converter_ACDC:Converter_ACDC_Hi-link_HLK-PMxx           |
| Q1–Q2   | S8050 Transistor      | Package_TO_SOT_THT:TO-92_Inline                          |
| R1–R8   | Resistors (1K / 10K)  | Resistor_SMD:R_0805_2012Metric                           |
| SW1–SW2 | Push Buttons          | Button_Switch_THT:SW_PUSH_6mm                            |
| U1      | ESP32-WROOM-32        | RF_Module:ESP32-WROOM-32                                 |
| U2–U3   | Optocoupler (PC817)   | Package_DIP:DIP-4_W7.62mm                                |
| U4      | AMS1117-3.3 Regulator | Package_TO_SOT_SMD:SOT-223-3_TabPin2                     |




![Schematic](WhatsApp%20Image%202025-06-17%20at%2014.48.11_e6d09a12.jpg)

