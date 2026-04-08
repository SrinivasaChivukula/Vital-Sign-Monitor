# Vital-Sign-Monitor 🏥

I built **Vital-Sign-Monitor** during a high-stakes hackathon (**HackWell**), where it actually took **1st Place**! It's a real-time computer vision system designed to keep a watchful eye on patients when hospital staff are stretched thin.

### 👁️ The Vision
Using **YOLOv8** (the gold standard for object detection), this system monitors patient presence and orientation in real-time. If it detects an emergency or a fall, it triggers immediate audio alerts and logs the event for medical review.

### ⚙️ How it’s built
- **Computer Vision:** YOLOv8n running at the edge for low-latency detection.
- **Backend Infrastructure:** A Python/Flask API that manages data flow from the camera to the DB.
- **Persistent Logging:** SQLite keeps a detailed history of every detection event.
- **Real-Time Alerts:** Asynchronous notification via `alert.wav` to ensure staff can react in seconds.

### 🚀 Try it out
1. `pip install -r requirements.txt`
2. `python src/run.py`

---
"Using AI to build a safer, more responsive healthcare system." 🚀
