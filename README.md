# 3d_printer
Quick start guide for 3d printer

# 3D Printer Quick Start Guide

This guide will walk you through installing OrcaSlicer, importing my tuned printer profile, connecting to the Raspberry Pi running Mainsail/Klipper, and changing Wi-Fi if needed.

---

## 1. Install OrcaSlicer
1. Go to [OrcaSlicer Releases](https://github.com/SoftFever/OrcaSlicer/releases).
2. Download the version for your OS:
   - **Windows:** `.exe`
   - **macOS:** `.dmg`
   - **Linux:** `.AppImage`
3. Install it.

---

## 2. Import My Printer Profile
1. Download [`profiles/OrcaSlicer_profile.3mf`](profiles/OrcaSlicer_profile.3mf).
2. In OrcaSlicer: `File` → `Import` → `Import Config Bundle`.
3. Select the profile file and confirm.

---

## 3. Change the Pi’s Wi-Fi Network
If you move the printer or change routers:
1. Power off the printer.
2. Remove the Pi’s micro-SD card.
3. Open it on your computer.
4. Edit [`wifi/mainsailos-wpa-supplicant.txt.example`](wifi/mainsailos-wpa-supplicant.txt.example) with your Wi-Fi name and password.
5. Save, eject, reinsert into Pi, and power on.

---

## 4. Connect to the Printer (Mainsail)
1. Connect your computer to the **same Wi-Fi** as the printer.
2. Open a browser and go to:
   - [http://mainsail.local](http://mainsail.local), or
   - The Pi’s IP address (`xxx.xxx.xxx.xxx`).
3. You’ll see the Mainsail dashboard.
4. Edit device in orcaslicer to set the device ip address 

---

## 5. Print a File
1. Slice your model in OrcaSlicer.
2. Click on send to device 

---



---

## 6. Tips
- Keep the bed clean with isopropyl alcohol.
- Run **Bed Mesh** in Mainsail after moving the printer.
- Preheat before loading filament.
