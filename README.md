# Vital-Sign-Monitor 🏥 👁️

Hey! **Vital-Sign-Monitor** is a real-time computer vision system designed to enhance patient safety through automated monitoring. It uses Deep Learning to track vital indicators and provides a centralized dashboard for real-time alerts.

## 🧐 What's the impact?
In high-stress medical environments, human observation can't be everywhere at once. This system acts as an "always-on" assistant that uses **YOLOv8** (You Only Look Once) to monitor patient presence and state, logging data directly to a persistent database and triggering audio-visual alerts if something seems off.

---

## 🛠 Engineering Stack
- **Computer Vision (YOLOv8):** Integrated state-of-the-art object detection to monitor patient state in real-time.
- **Backend (Flask & Python):** Built a RESTful API to bridge the gap between the vision engine and the user interface.
- **Data Persistence (SQLite):** Logged all "events" into a `vision_data.db` for historical analysis and reporting.
- **Real-Time Alerts:** Implemented an asynchronous alerting system using `alert.wav` to ensure zero-latency notification for staff.
- **Frontend Dashboard:** A clean UI that displays live detection logs and system health.

---

## 📊 Performance
The system is optimized to run on edge devices, maintaining high FPS while processing frame-by-frame detection.

---

## 🚀 How to Run
1. **Clone the Repo:**
   ```bash
   git clone https://github.com/SrinivasaChivukula/Vital-Sign-Monitor.git
   cd Vital-Sign-Monitor
   ```
2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Ignition:**
   ```bash
   python src/run.py
   ```

---

## 📂 Project Structure
- `src/`: Core logic including the vision engine (`monitor_server.py`) and the API (`backend_api.py`).
- `assets/`: Contains the pre-trained **YOLOv8n** model and notification assets.
- `frontend/`: The dashboard source code.
- `vision_data.db`: The persistent event log.

---

## 🧠 Strategic Takeaways
- **AI at the Edge:** Learned how to deploy deep learning models in real-time environments without sacrificing speed.
- **Full-Stack AI:** Built every layer from the raw pixel input to the final UI dashboard.
- **Safety-Critical Design:** Focused on building a reliable alerting mechanism for high-stakes environments.

---

## 👨‍💻 Author
**Srinivasa Chivukula**  
*Computer Science Major | AIML, CyberSecurity, and Cloud Technologies*

---
"AI for a safer, healthier world." 🚀
