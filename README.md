# ULCSRWLEDC
Ultra Low Cost Sound Reactive WLED Controller

## Features

- Small size
- Cheap components
- ICS-43434 MEMS Microphone (optional)
- MOSFET as "Relay"
- Mini Blade Fuse
- Solder Pads instead of Screw Terminal Blocks

![Rendered picture of pcb](https://github.com/NandXor96/ULCSRWLEDC/blob/main/render.png?raw=true)

## BOM

| Reference | Value | Comment | Estimated Cost per piece |
|---|---|---|---|
| C1, C6 | 100nF | MLCC 0805 | 0.01€ |
| C2, C3, C4* | 22uF | MLCC 0805 | 0.10€ |
| C5 | 1uF | MLCC 0805 | 0.05€ |
| C7 | >330uF | Electrolytic Cap D8.0 P3.5 | 0.15€ |
| D1 | SS14 | Schottky | 0.05€ |
| F1 | 2 - 10A | Mini Blade Fuse | 0.50€ |
| MK1** | ICS43434 | optional MEMS Microphone | 0.95 - 2.90€ |
| Q1 | - | SOIC-8 PMOS according to your needs - f.e. IRF7410 | 0.70 - 1.50€ |
| Q2 | - | SOT-23-3 NMOS according to your needs - f.e. IRLML6244 | 0.05 - 0.50€ |
| R1, R3, R4, R7 | 10k | 0805 Resistor | 0.01€ |
| R4 | 100k | 0805 Resistor | 0.01€ |
| R6 | 300R | 0805 Resistor | 0.01€ |
| R2* | 0.03-1R | optional 0805 Resistor | - |
| SW1 | - | Reset Switch SMD 6x3.5mm - f.e. PTS636 | 0.05 - 0.50€ |
| U1 | AMS1117-3.3 | SOT-223-3 LDO | 0.05 - 0.50€ | 
| U2 | ESP-WROOM-32 | With antenna | 2.85€ |
| PCB | - | JLCPCB | 1.20€ |
|------|------|------|------|
|  |  |  | 5.12 - 10.89€ |

*If you have problems with the stability of the LDO you have two options:
1. Cut the trace resistance between R2 and try some 0805 resistors from 0.03-1ohm.
2. Choose tantal for C4 and bridge R2

** You can build it without the microphone. Then you don't need C6, R4 and MK1.

## Assembly

To assemble the PCB, I recommend using a hot plate or soldering oven for the upper side, and hand-soldering for the ESP32 on the back.
**Preheat** the PCB before soldering anything by hand and use a **powerful soldering iron**!  
Do NOT use a very small tip!

## Disclaimer

The circuit board provided on this GitHub repository is offered "as is," without any warranties or guarantees of any kind. By accessing and utilizing this circuit board, you acknowledge and agree that you do so at your own risk.

The creator and contributor of this repository, shall not be held responsible or liable for any damages, losses, or injuries that may occur as a result of building and / or using this circuit board. This includes but is not limited to any direct, indirect, consequential, or incidental damages.
