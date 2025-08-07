# low-noise-amplifier-jfet150
Open source low-noise amplifier project using JFET150

# 🔊 Low-Noise Amplifier (LNA) Project – JFET150 + OPA211 + Differential Stage

This project documents the design and testing of a **low-noise amplifier (LNA)**, based on a JFET input stage followed by a precision op-amp (OPA211), and a second-stage differential amplifier.

Everything is **open source** and shared for learning, experimentation, and collaboration.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Circuit Design](#circuit-design)
- [Measurements](#measurements)
- [Bill of Materials](#bill-of-materials)
- [Schematic and PCB](#schematic-and-pcb)
- [Usage](#usage)
- [License](#license)
- [Author](#author)

---

## 🔍 Overview

This two-stage amplifier is designed for applications requiring ultra-low noise and high gain:

1. **Low-noise preamp** based on a JFET transistor (JFET150) + OPA211 with ~40 dB gain
2. **Differential amplifier** that adds another 20 dB gain and rejects common-mode noise

---

## ⚙️ Features

| Parameter              | Value                  |
|------------------------|------------------------|
| Total Gain             | ~60 dB (×1000)         |
| Input Noise            | [2 nV/√Hz, @1kHz]      |
| Bandwidth              | [10 Hz – 100 kHz]      |
| Supply Voltage         | 0V-5V                  |
| Input Impedance        | >? MΩ                  |
| Output Impedance       | ~??? Ω                 |

---

## 🔧 Circuit Design

### 🔹 Stage 1 – Low-Noise Preamp

- JFET input (JFET150)
- Precision Op-Amp (OPA211)
- Gain: ~40 dB
- Focus: low noise, high input impedance

### 🔸 Stage 2 – Differential Amplifier

- Differential op-amp topology
- Gain: ~20 dB
- Focus: common-mode noise rejection

---

## 📊 Measurements


The FFT screenshots, oscilloscope captures, etc. are under `measurements/` folder.

---

## 🖨️ Schematic and PCB

- [ ] Schematic in KiCad / Eagle / LTspice
- [ ] PCB layout
- [ ] Gerber files for fabrication
- [ ] 3D render (optional)

Images and files are into the `hardware/` directory.

---

## 🔌 Usage

1. **Power Supply**: +5 V regulated
2. **Input**: Search Coil (a magnetometer)
3. **Output**: Connect to oscilloscope or ADC

> ⚠️ Make sure to use a proper power supply with current limiting

---

## 🪪 License

This project is licensed under the **MIT License** – see the [LICENSE](./LICENSE) file for details.

---

## 🙋 Contributions

Feel free to fork, open issues, or submit pull requests if you want to improve or adapt this project.

---

## 👨‍🔬 Author

Designed by Li Jiajing, This project was carried out during an assistant engineer internship under the supervision of Alexis Jeandet at the Plasma Physics Laboratory (LPP).

---

