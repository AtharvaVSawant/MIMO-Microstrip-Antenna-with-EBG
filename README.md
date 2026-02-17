# MIMO-Microstrip-Antenna-with-EBG
Design and fabrication of a 2×1 MIMO patch antenna with low mutual coupling using Electromagnetic Bandgap (EBG) structures, operating at 2.4 GHz for 5G and next‑generation wireless networks.

# MIMO Patch Antenna with Low Mutual Coupling for Next Generation Wireless Networks
![Mimo 1](https://github.com/user-attachments/assets/1efb65ba-f5da-4004-8aa5-66ac8959e6dc)

![Antenna Prototype](photos/antenna_front.jpg)  
*Figure: Fabricated MIMO antenna with EBG structure*

## 📡 Project Overview

This project presents the design, simulation, fabrication, and testing of a compact **2×1 MIMO patch antenna** operating at **2.4 GHz** (ISM band) with significantly reduced mutual coupling. An **Electromagnetic Bandgap (EBG)** structure is integrated between the radiating elements to suppress surface waves and improve isolation.

The antenna is designed on an FR4 substrate (ε<sub>r</sub> = 4.4, thickness = 1.6 mm) and is suitable for next-generation wireless applications such as **5G, IoT, smart devices, and Wi-Fi/Bluetooth integration**.

**Key achievements:**
- Return loss (S11) < -35 dB at resonance
- Isolation (S21) improved from -17.72 dB to **-32.17 dB** using EBG
- Average gain increased from -25.22 dB to **-2.69 dB**
- Communication range extended from 3.5 m to **520 m** (Friis equation estimate)

---

## 📁 Repository Contents

| Folder/File | Description |
|-------------|-------------|
| `report/` | Full B.Tech project report (PDF) |
| `simulation/` | HFSS simulation files |
| `fabrication/` | PCB layouts  |
| `photos/` | Simulation results |
| `results/` | Measured S-parameter data (CSV format) |
| `README.md` | This file |

---

## 🔧 Design Specifications

| Parameter | Value |
|-----------|-------|
| Frequency | 2.4 GHz |
| Substrate | FR4 epoxy |
| Dielectric constant (ε<sub>r</sub>) | 4.4 |
| Substrate thickness | 1.6 mm |
| Patch dimensions (each) | 36.1 mm × 27.4 mm |
| EBG unit cell size | 14.1 mm × 14.1 mm |
| Number of EBG cells | 3 (arranged vertically) |
| Feeding | Coaxial probe feed |
| MIMO configuration | 2×1 linear array |

---

## 📊 Key Results

### Simulation Comparison (with vs. without EBG)

| Parameter | Without EBG | With EBG |
|-----------|-------------|----------|
| Resonant frequency | 2.400 GHz | 2.460 GHz |
| Return loss (S11) | -30.87 dB | **-35.42 dB** |
| Mutual coupling (S21) | -17.72 dB | **-32.17 dB** |
| Max gain | -22.48 dB | **0.00 dB** |
| Average gain | -25.22 dB | **-2.69 dB** |
| Estimated range (Friis) | 3.5 m | **520 m** |

### Radiation Pattern
- The EBG structure dramatically improves radiation directivity and efficiency.
- Surface wave suppression is clearly visible in current distribution plots.

### Measured Results (with EBG)
- S11 < -15 dB across 2.4–2.5 GHz
- S21 < -25 dB across the band
- Good agreement with simulations (see `results/` folder)

---

## 🛠️ Fabrication Process

The antenna was fabricated using **PCB etching** (ExpressPCB method):
1. Layout designed in ExpressPCB software.
2. Printed on glossy paper using laser printer.
3. Transferred to copper-clad board via heat (iron).
4. Etched in ferric chloride solution.
5. Drilled and soldered SMA connectors.

See `fabrication/` for PCB layouts and `photos/` for step-by-step images.

---

## 📐 Simulation Tools

- **ANSYS HFSS 2023 R2** – Full-wave electromagnetic simulation
- **ExpressPCB** – PCB layout design

---

## 🧪 Testing Setup

- **Vector Network Analyzer (VNA)** – Used to measure S-parameters (S11, S21)
- Calibration: SOLT (Short-Open-Load-Through) before each test
- Environment: Non-metallic platform, minimal reflections

Measured data is available in `results/`.

---

## 🚀 Applications

- 5G and beyond wireless systems
- MIMO arrays for base stations and user equipment
- IoT devices, smart home, wearables
- Wi-Fi 6/6E, Bluetooth integration
- Smart city infrastructure

---

## 🔮 Future Scope

- Integration with reconfigurable/metasurface designs
- AI-optimized geometry for multi-band operation
- Use of low-loss substrates for higher efficiency
- Beamforming and massive MIMO extensions

---

## 👥 Authors

- **Shrisha Jayen Kokku** 
- **Shreyash Shyamsundar Koli** 
- **Yash Sanjeev Naik** 
- **Atharva Vinod Sawant** 

**Under the guidance of:**  
Dr. Pramod P. Bhavarthe  
*Associate Professor, Department of Electronics & Telecommunication Engineering*  
Shah & Anchor Kutchhi Engineering College, Mumbai

---

## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

We thank our guide Dr. Pramod P. Bhavarthe for his invaluable support, the Department of Electronics & Telecommunication Engineering, and the college management for providing resources and encouragement.

---

## 📬 Contact

For any queries, please contact:  
atharvasawant3183@gmail.c0m 
https://www.linkedin.com/in/atharvavsawant/

---

## 📚 References

Key references are listed in the project report (`report/Btech_Major_Project_Report.pdf`).  
Some important ones:

1. F. Yang and Y. Rahmat-Samii, "Microstrip antennas integrated with electromagnetic band-gap (EBG) structures," *IEEE Trans. Antennas Propag.*, 2003.
2. I. Nadeem and D. Choi, "Study on mutual coupling reduction technique for MIMO antennas," *IEEE Access*, 2019.
3. C. K. Ghosh et al., "Mutual coupling reduction of microstrip MIMO antenna using microstrip resonator," *Wireless Personal Communications*, 2020.
