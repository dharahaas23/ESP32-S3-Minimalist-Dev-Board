# ESP32-S3-Minimalist-Dev-Board
A compact 2-layer ESP32-S3 development board with USB-C, CH340K USB-to-TTL,  AMS1117 3.3V regulator, antenna keep-out zone, and full GND fill.  Designed in KiCad. DRC clean. Production-ready gerbers included.

![3D Render](https://github.com/user-attachments/assets/1757e43f-507d-452e-be81-71649e9b303b)
![3D Render](https://github.com/user-attachments/assets/5b21775f-d727-421b-8677-7545e2163080)

## Features

- **MCU:** ESP32-S3 WROOM-32 module
- **USB:** USB-C connector with CH340K for USB-to-TTL communication
- **Power:** AMS1117-3.3V onboard voltage regulator
- **GPIO:** 10 broken-out IO pins (IO1–IO9 + GND, 3.3V, 5V)
- **Controls:** Dedicated BOOT and RESET push buttons
- **Layers:** 2-layer PCB
- **Ground Plane:** Full GND fill on both layers for noise reduction
- **Antenna:** Keep-out zone correctly implemented for RF clearance
- **DRC:** 0 errors, 0 warnings

## PCB Layout

![PCB Layout](https://github.com/user-attachments/assets/c99972a6-f46b-402f-b40a-15c6076ea1a1)
![PCB Layout](https://github.com/user-attachments/assets/c99972a6-f46b-402f-b40a-15c6076ea1a1).

## Schematic

The design includes 5 functional blocks:
- USB-C input
- CH340K USB-to-TTL bridge
- AMS1117 3.3V voltage regulation
- ESP32-S3 WROOM-32 module
- GPIO breakout headers + Boot/Reset

![Schematic](https://github.com/user-attachments/assets/ef9f2253-3c5d-4960-b4f0-982f9bb06600)

## Design Decisions

- **CH340K** chosen over CP2102 for cost efficiency and wide driver support
- **Keep-out zone** placed over antenna area to prevent copper interference 
  with RF performance
- **GND fill** on both F.Cu and B.Cu layers for EMI reduction and thermal 
  dissipation
- **AMS1117** decoupling capacitor placed close to output pin

## Files

| File | Description |
|------|-------------|
| `[esp 32 smaller.zip](https://github.com/user-attachments/files/27808006/esp.32.smaller.zip)[Uploading esp 32 smaller.kicad_sch…]()
` | Production-ready Gerber files |
| `schematic.pdf` | Full schematic export |
| `bom.csv` | Bill of materials |

## Manufacturing

Designed for fabrication at JLCPCB / PCBWay:
- Board size: ~45 x 26 mm (2-layer)
- Min trace width: 0.25 mm
- Via drill: 0.8 mm

## Tools Used

- KiCad 10.0
- ESP32-S3 WROOM-32 datasheet for antenna keep-out dimensions
- AMS1117 datasheet for decoupling recommendations

## Author

**Simhadri Dharahaas**  
ECE Undergraduate | Embedded Systems & PCB Design  
[LinkedIn](https://www.linkedin.com/in/dharahaas-simhadri-b17b4b358?utm_source=share_via&utm_content=profile&utm_medium=member_android)
