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

The transfer function measurements were performed using two 20 dB attenuators, resulting in a total attenuation of 33 dB applied to the gain:

This is the transfer function of the first stage (blue curve):
![Amplification 1st stage](measurements/Amplification_1st_stage.png)

This is the transfer function of the second stage:
![Amplification 2nd stage](measurements/Amplification_2nd_stage.png)

And there we have the input noise of the amplifier
![Input noise](measurements/Input_Noise.png)


---

## 🖨️ Schematic and PCB

Browse PCB and schematics online [here](https://kicanvas.org/?github=https%3A%2F%2Fgithub.com%2FJiajing-Li-2003%2Flow-noise-amplifier-jfet150%2Fblob%2Fmain%2Fhardware%2Fampli%2520jfe150%2520searchcoil.kicad_pro).


Files are in the `hardware/` directory.

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
