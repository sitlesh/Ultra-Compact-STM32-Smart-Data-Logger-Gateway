
# Custom Embedded Controller Board with Micro SD Storage

A professionally designed, compact **2-layer printed circuit board (PCB)** developed using **KiCad 8.0**. This hardware platform is engineered for standalone embedded applications requiring localized data logging, high-precision timing, and robust power delivery.

---

## 📸 Hardware Showcase

### 🏷️ 3D Render Preview
<img width="3450" height="1886" alt="Ultra-Compact STM32 Smart Data Logger   Gateway" src="https://github.com/user-attachments/assets/e93fce8e-a7f3-4897-bf2d-54b6753bd6fd" />

### 🗺️ Board Layout (Top & Bottom View)
| Top Copper Layer (F.Cu) | Bottom Copper Layer (B.Cu) |
| :---: | :---: |
| <img width="2328" height="1468" alt="Screenshot (32)" src="https://github.com/user-attachments/assets/001ac98b-54e7-4652-a6db-91f2745bf4fb" /> | <img width="2312" height="1473" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/a3baccfd-a89d-49fd-932c-f3221c77ac5a" /> |

---

## 🚀 Key Hardware Features

* **Micro SD Card Slot (J4):** Wired via high-speed SPI interface. Features localized decoupling, direct short-return paths to ground, and integrated mechanical shield grounding (`SH GND`) to suppress ESD and EMI.
* **Dual-Clock Architecture:** * **High-Speed Crystal (Y1 - 8MHz):** Provides a stable external clock source for the primary microcontroller core, stabilized by 20pF loading capacitors.
  * **Low-Speed RTC Crystal (Y2 - 32.768kHz):** Dedicated ultra-low-power crystal with 10pF loading capacitors for precise time-stamping.
* **Power Management:** Heavy-duty 2-position screw terminal (`J1`) for power input, protected by a robust on-board Schottky/Rectifier Diode (`D1`) for reverse polarity protection.
* **Signal Integrity:** Utilizes duplicated, stitched copper zones (`GND`) across both layers to maximize thermal dissipation, lower loop inductance, and suppress high-frequency noise.

---

## 📁 Repository Directory & File Descriptions

This repository contains all the native design assets and manufacturing files required to replicate or modify this project.

### 🛠️ Source Design Files (KiCad 8.0)
* **[`Ultra-Compact STM32 Smart Data Logger & Gateway.kicad_pro`](./Ultra-Compact%20STM32%20Smart%20Data%20Logger%20%26%20Gateway.kicad_pro)** : The master KiCad project file that links the schematic and PCB layout configurations together.
* **[`Ultra-Compact STM32 Smart Data Logger & Gateway.kicad_sch`](./Ultra-Compact%20STM32%20Smart%20Data%20Logger%20%26%20Gateway.kicad_sch)** : The complete schematic capture. Contains the logical circuit connections, component symbols, and electrical nets.
* **[`Ultra-Compact STM32 Smart Data Logger & Gateway.kicad_pcb`](./Ultra-Compact%20STM32%20Smart%20Data%20Logger%20%26%20Gateway.kicad_pcb)** : The physical 2-layer board layout, trace routing, component footprints, and copper ground planes.
* **[`gitignore.txt`](./gitignore.txt)** : Configured to exclude local KiCad auto-saves and temporary backup files to keep the repository clean.

### 📦 Manufacturing Files
* **[`Download Pre-packaged Gerbers ZIP (Gerbers.zip)`](./Gerbers.zip)** : Contains the combined ZIP archive. Click this link and hit the **Download** button on the next page to get all production-ready Gerber and Drill files for direct manufacturing.

---

## ⚙️ Fabrication Specifications

| Parameter | Specification |
| :--- | :--- |
| **Material Type** | FR-4 Standard |
| **Layer Count** | 2 Layers |
| **Board Thickness** | 1.6 mm |
| **Copper Weight** | 1 oz (35μm) outer layers |
| **Surface Finish** | HASL (with lead) or ENIG |
| **Solder Mask** | User Preference (Green/Blue/Black) |
| **Silkscreen** | White (High contrast) |

---

## 📝 License
This hardware design is open-source. Feel free to clone, modify, and build upon it for your own custom applications.
