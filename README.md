# sensor-data-from-the-latest-final-assignment
Source code and test data for an Air Quality Monitoring System in Indonesian volcanic areas. This project evaluates hazardous gas sensors and LoRa 433MHz transmission to mitigate exposure risks.
# 🌋 Air Quality Monitoring System in Volcanic Areas

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Hardware](https://img.shields.io/badge/Hardware-ESP32%20%7C%20LoRa%20433MHz-orange.svg)

## 📌 Project Overview
This repository contains the source code, hardware schematics, and test data for an **Air Quality Monitoring System** specifically designed for volcanic regions in Indonesia. The system aims to mitigate the risk of exposure to hazardous gases by providing real-time data monitoring using long-range radio communication.

This project is a final academic assignment and focuses on two main evaluations:
1. **Sensor Accuracy and Reading Tests:** Evaluating the precision of hazardous gas sensors in simulated/real environments.
2. **LoRa 433MHz Transmission Tests:** Measuring data transmission speed, packet loss, and reliability over various distances.

## 🛠️ Hardware & Technology Stack
* **Microcontroller:** [Insert Microcontroller, e.g., ESP32 / Arduino Uno]
* **Communication:** LoRa Module (433MHz)
* **Sensors:** [Insert Sensors, e.g., MQ-135, MQ-7, etc.]
* **Software/Platform:** [Insert Platform, e.g., Arduino IDE, ThingsBoard, etc.]
## 1.0 Sensor Calibrating

During the calibration phase, environmental conditions (Temperature & Humidity) and the resistance (Rs) of various gas sensors (MEMS, MQ7, MQ136, MQ135) were recorded. The table below represents a cross-section sample of the dataset, showcasing different testing intervals for each sensor group.

### Data Sample

| No | Time | Suhu (°C) | Kelembapan (%) | Vo MEMS | Rs MEMS | Vo MQ7 | Rs MQ7 | Vo MQ136 | Rs MQ136 | Vo MQ135 | Rs MQ135 |
|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|
| 1 | 21:13:16 | 22.00 | 89.74 | 1.39 | 13.63 | - | - | - | - | - | - |
| 2 | 21:13:45 | 22.00 | 89.74 | 1.37 | 13.94 | - | - | - | - | - | - |
| 58 | 22:43:10 | 21.71 | 90.72 | - | - | 0.73 | 9.81 | 0.10 | 88.89 | - | - |
| 59 | 22:43:15 | 21.71 | 90.72 | - | - | 0.73 | 9.84 | 0.10 | 88.89 | - | - |
| 115 | 23:02:51 | 21.58 | 91.05 | - | - | - | - | - | - | 0.10 | 88.89 |
| 116 | 23:02:56 | 21.58 | 91.05 | - | - | - | - | - | - | 0.10 | 88.89 |

> *Note: The dataset was recorded in sequential phases. Empty values (`-`) indicate that the respective sensor was not active or being recorded during that specific timeframe.*

### Calibration Resistance (Rs) Chart
The following chart visualizes the fluctuation of the sensors' resistance (Rs) over time during the calibration process.

![Sensor Calibration Chart](docs/Hasil Pembacaan Kalibrasi Sensor Rs dan Vo Terhadap Suhu Dan Kelembapan.png)
