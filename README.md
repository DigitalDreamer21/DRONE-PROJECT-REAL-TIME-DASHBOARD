# 🚁 Real-Time Drone Surveillance Dashboard

An **AI-powered real-time drone monitoring dashboard** that streams live video, detects people using **YOLOv8**, and visualizes drone telemetry such as GPS, altitude, battery, and signal strength. This project demonstrates real-world skills in **computer vision, real-time systems, and full-stack development**, designed to meet **industry and placement standards**.

---

## 📌 Project Overview

Modern drone applications require **real-time awareness, accuracy, and reliability**. This project simulates a **real-time drone surveillance system** capable of:

* Streaming live video from an IP camera / drone feed
* Detecting people in real time using deep learning (YOLOv8)
* Displaying live telemetry data on a web dashboard
* Handling continuous data flow with low latency

The system is built with a **modular and scalable architecture**, similar to what is used in real-world surveillance and monitoring platforms.

---

## ✨ Key Features

* 📡 **Live Video Streaming** from drone/IP camera
* 🧠 **Real-Time Person Detection** using YOLOv8
* 📍 **GPS-based Target Localization** (simulated mapping)
* 📊 **Drone Telemetry Visualization**

  * Battery level
  * Altitude
  * Signal strength
* 🟢 **Radar-Style Proximity View** for detected persons
* ⚡ **Low-Latency Communication** using Socket.IO
* 🧩 **Multithreaded Processing** for smooth performance

---

## 🛠️ Tech Stack

### Backend

* **Python**
* **Flask** – Web server
* **Flask-SocketIO** – Real-time communication
* **OpenCV** – Video processing
* **Ultralytics YOLOv8** – Person detection
* **Threading** – Parallel frame capture & detection

### Frontend

* **HTML5, CSS3, JavaScript**
* **Socket.IO Client** – Live updates

### AI / Computer Vision

* **YOLOv8 (yolov8n)**
* Real-time inference on video frames

---

## 🧠 System Architecture

1. Drone/IP camera streams MJPEG video
2. Backend captures frames in real time
3. YOLOv8 processes selected frames for person detection
4. Detection results + telemetry are packaged as JSON
5. Data is streamed to the frontend using Socket.IO
6. Dashboard updates live without page refresh

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/DigitalDreamer21/DRONE-PROJECT-REAL-TIME-DASHBOARD.git
cd DRONE-PROJECT-REAL-TIME-DASHBOARD
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Configure IP Camera / Drone Feed

Edit `app.py`:

```python
ip_cam = "http://<your-ip-camera-stream>"
```

### 4️⃣ Run the Application

```bash
python app.py
```

### 5️⃣ Open in Browser

```
http://localhost:8080
```

---

## 📂 Project Structure

```
├── app.py              # Flask application & Socket.IO server
├── detector.py         # YOLOv8 detection & video processing logic
├── yolov8n.pt          # YOLOv8 pretrained model
├── templates/
│   └── index.html      # Dashboard UI
├── static/             # CSS / JS assets
├── requirements.txt    # Project dependencies
└── README.md
```

---

## 🎯 Use Cases

* Drone-based surveillance systems
* Smart city monitoring
* Disaster management & rescue operations
* Border & perimeter security
* AI-based defense and monitoring solution

## 🙌 Author

**DigitalDreamer21**
Aspiring AI / Computer Vision Engineer

