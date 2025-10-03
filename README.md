# 🔥 PyroGuard

**AI-Powered Fire & Temperature Monitoring System**
*By Vishali T & Vijaya Pradhap S V*

---

## 📌 Overview

PyroGuard is a **smart fire and temperature monitoring system** designed to provide **early fire hazard detection and alerts**.
It integrates **YOLOv5-based AI fire detection** with **ESP32 temperature sensing** and a **web dashboard**, offering real-time insights and alerts to ensure safety in critical environments.

---

## ✨ Features

* 🔎 **YOLOv5 Fire Detection** – AI model trained to detect fire in real-time.
* 🌡 **ESP32 with Temperature Sensor** – monitors environment continuously.
* 🎛 **Rotary Encoder Threshold Control** – adjust alert levels dynamically.
* 🌐 **Web Dashboard** – live fire detection feed & sensor monitoring.
* ⚡ **Instant Alerts** – immediate warnings when fire or abnormal temperatures are detected.

---

## 🏗 System Architecture

```
ESP32 (Sensor + Encoder)
        ↓
   Flask Backend (YOLOv5 + API)
        ↓
   Web Dashboard (HTML/CSS/JS)
```

---

## 📂 Project Structure

```
pyroguard/
│
├── backend/                # Flask + YOLOv5 backend
│   ├── app.py
│   ├── fire_win.pt
│   └── requirements.txt
│
├── esp32/                  # ESP32 code
│   └── esp32_code.ino
│
├── webpage/                # Frontend files
│   └── index.html
│
├── docs/                   # Reports, posters, documentation
│   └── mini_project_report.pdf
│
├── LICENSE
└── README.md
```

---

## 🚀 Getting Started

### 🔧 Prerequisites

* Python 3.8+
* ESP32 with Arduino IDE / PlatformIO
* Flask, Torch, OpenCV, requests
* Pretrained YOLOv5 fire detection model (`fire_win.pt`)

### 📥 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/<your-username>/pyroguard.git
   cd pyroguard
   ```

2. **Install backend dependencies**

   ```bash
   pip install -r backend/requirements.txt
   ```

3. **Run Flask backend**

   ```bash
   python backend/app.py
   ```

4. **Flash ESP32**

   * Open `esp32/esp32_code.ino` in Arduino IDE
   * Add WiFi credentials
   * Upload to ESP32

5. **Start dashboard**

   * Open `webpage/index.html` in a browser
   * Monitor live detection & temperature data

---

## 📊 Demo

(Add screenshots, circuit images, or demo video links here)

---

## 👩‍💻 Contributors

* **Vishali T**
* **Vijaya Pradhap S V**

---

## 📜 License

This project is licensed under the **MIT License** – feel free to use, modify, and distribute.

---

## ⭐ Acknowledgements

* [Ultralytics YOLOv5](https://github.com/ultralytics/yolov5)
  
