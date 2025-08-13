# Non-Destructive Testing System for Milk Quality

This project presents a low-cost, portable system for detecting water adulteration in milk using **microwave sensing** and **software-defined radio (SDR)** technology.  
By leveraging the **ADALM-PLUTO SDR**, **Raspberry Pi**, and a **custom-designed microwave resonator**, the device measures dielectric property variations to determine water content without damaging the sample.

---

## Project Video
- Making of the Sensor: [Watch Here](https://drive.google.com/file/d/1Vm7-oqjqp5PHV5cjzx6X19xbDVr_Dte7/view?usp=drive_link)

---

## Key Features
- Detects **water content percentage** in milk with high sensitivity.
- **Non-destructive** and contact-based dielectric measurement.
- Operates at **2.4 GHz ISM band** using a custom SRR-based microwave sensor.
- Real-time data acquisition and processing with a **Python GUI**.
- Portable and low-cost for **field deployment**.

---

## System Overview
1. **Microwave Sensor Design**  
   - Nested square split ring resonators (SRRs) fabricated on Rogers RO4350B substrate.  
   - Optimized in CST Microwave Studio for high sensitivity to dielectric changes.

2. **Signal Processing**  
   - ADALM-PLUTO SDR excites the sensor and measures the **S21 transmission coefficient**.  
   - Raspberry Pi handles data acquisition and processing via **pyadi-iio**.

3. **Liquid Classification**  
   - Attenuation levels are mapped to specific milk-water ratios.  
   - GUI displays results every 3 seconds.

---

## Hardware Used
- ADALM-PLUTO SDR
- Raspberry Pi
- Custom microwave resonator sensor
- SMA connectors & RF cables

---

## Software & Tools
- CST Microwave Studio
- Python (Tkinter, NumPy, pyadi-iio)
- Vector Network Analyzer (for calibration)

---

## Applications
- Milk adulteration detection in dairy farms and collection centers
- Field-deployable liquid quality testing
- Scalable to detect other liquid adulterants
