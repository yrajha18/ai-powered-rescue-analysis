# 🚁 Fury Fly – AI Powered Rescue Drone System

## 📌 Overview

**Fury Fly** is an AI-powered micro-drone rescue assistance system designed for **disaster environments where GPS signals are unavailable**, such as collapsed buildings, mines, or indoor disaster zones.

The system uses **computer vision and artificial intelligence** to detect trapped survivors, track individuals uniquely, and prioritize rescue operations based on risk and visibility conditions.

Our goal is to provide **fast, low-cost, and intelligent rescue support** for first responders during emergency situations.

---

# 🎯 Problem Statement

During disasters like **earthquakes, building collapses, fires, or mine accidents**, rescuers face several challenges:

* Limited visibility
* No GPS signals indoors
* Difficulty locating survivors quickly
* Risk of secondary collapse
* Large areas to search manually

Traditional rescue methods can be **slow, dangerous, and inefficient**.

---

# 💡 Our Solution

**Fury Fly** is a **compact AI-enabled drone system** capable of:

* Detecting humans using computer vision
* Tracking unique individuals using visual identification
* Prioritizing rescue targets using a dynamic risk score
* Providing real-time analytics through a dashboard
* Giving voice alerts when new survivors are detected

The system helps rescuers **quickly identify and prioritize trapped survivors**.

---

# 🧠 Key Features

### 👤 AI Human Detection

Uses **YOLOv8 object detection** to detect humans in real-time from camera feeds.

### 🧬 Person Re-Identification

A custom **visual matching system** ensures that the same person is **not counted multiple times**.

Features used:

* Color histogram analysis
* Regional color segmentation
* Structural similarity comparison
* Motion tracking

### ⭐ Rescue Priority System

Each detected person is assigned a **priority score** based on:

* Distance from camera
* Confidence of detection
* Environmental risk conditions
* Position within the frame

This helps rescue teams **focus on the most critical survivors first**.

### 📊 Real-Time Dashboard

The system provides a **live rescue dashboard** displaying:

* Total unique persons detected
* Current persons in view
* Detection statistics
* Priority list of survivors
* Risk level estimation

### 🔊 Voice Alert System

When a **new survivor is detected**, the system announces it using **text-to-speech alerts**.

Example:

> "New person detected. Total unique persons: 3"

---

# 🏗 System Architecture

```
Camera / Drone Feed
        │
        ▼
   YOLOv8 AI Model
   (Human Detection)
        │
        ▼
Person Re-Identification
        │
        ▼
Priority Score Calculation
        │
        ▼
Rescue Dashboard + Alerts
```

---

# ⚙️ Technology Stack

### Programming

* Python

### Computer Vision

* OpenCV

### AI / Machine Learning

* YOLOv8 (Ultralytics)

### Interface

* Tkinter Dashboard

### Additional Libraries

* NumPy
* PyTTSX3 (Voice alerts)
* Scikit-image (Image similarity)

---

# 📦 Project Structure

```
FURY-FLY
│
├── rescue_system.py
├── requirements.txt
├── README.md
│
├── fury-india
│   ├── CMakeLists.txt
│   └── sdkconfig
│
└── ESP32Drone_Firmware_FlashdownloadTool_0x00.bin
```

---

# 🚀 Installation

### 1️⃣ Clone the repository

```
git clone https://github.com/yrajha18/ai-powered-rescue-analysis.git
cd ai-powered-rescue-analysis
```

---

### 2️⃣ Install dependencies

```
pip install -r requirements.txt
```

---

### 3️⃣ Download YOLO model

The system uses:

```
yolov8n.pt
```

Ultralytics will automatically download it when running the program.

---

### 4️⃣ Run the system

```
python rescue_system.py
```

---

# 📷 Camera Setup

The project supports:

* IP camera
* Phone camera
* Drone camera feed

Example camera URL:

```
http://10.54.46.12:4747/video
```

You can stream using apps like **DroidCam or IP Webcam**.

---

# 📊 Example Output

The system displays:

* Bounding boxes around detected persons
* Unique person IDs
* Priority scores
* Rescue risk indicator
* FPS performance metrics

---

# 🎥 Demo Scenario

Possible use cases include:

* Earthquake rescue operations
* Building collapse search
* Mine accident response
* Indoor disaster environments
* Fire rescue missions

---

# 🧪 Future Improvements

Planned upgrades include:

* Thermal camera integration
* Multi-drone coordination
* DeepSORT tracking
* Survivor pose estimation
* SOS gesture detection
* Offline edge AI deployment

---

# 🏆 Hackathon Value Proposition

### Our USP

* **Low-cost micro drone solution**
* **Works in GPS-denied environments**
* **Real-time AI survivor detection**
* **Unique person identification**
* **Priority-based rescue decision system**

This makes Fury Fly a **practical and scalable disaster-response technology**.

---

# 👨‍💻 Team

**Team Name:** The Risers

**Project:** Fury Fly – AI Powered Rescue System

---

# 📜 License

This project is open source and available under the **MIT License**.

---

# ❤️ Acknowledgements

Special thanks to:

* Ultralytics YOLOv8
* OpenCV Community
* Python Open Source Ecosystem

---

# 🌍 Vision

Our vision is to build **AI-powered rescue systems that help save lives during disasters**.

Technology should not only be powerful — it should be **life-saving**.
