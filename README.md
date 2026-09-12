# Worker-Safety-Monitoring-System

## 🚧 AI Worker Safety Monitoring System | Day 1

Started building an **AI-powered Worker Safety Monitoring System** focused on improving workplace safety through real-time computer vision.

### ✅ Phase 1: Environment Setup Completed

Today I completed the complete development environment and project foundation.

### 🛠️ Technologies Set Up

* Python 3.13.5
* YOLO / Ultralytics
* OpenCV
* NumPy
* Flask
* Pygame
* Python-dotenv

### 📁 Project Structure Created

```text
AI-Worker-Safety-System/
│
├── venv/
├── models/
├── detection/
├── safety/
├── alarm/
├── camera/
├── dashboard/
├── database/
├── logs/
├── snapshots/
├── utils/
├── static/
├── tests/
├── .gitignore
├── requirements.txt
└── test_environment.py
```

### 🔍 Environment Validation

Verified that the core libraries are working correctly:

```text
OpenCV       : OK
NumPy        : OK
Pygame       : OK
Flask        : OK
Ultralytics  : OK
YOLO         : OK
```

### 🎯 Project Objective

The system will eventually monitor workers through a camera and determine whether they are wearing the required safety equipment:

* 🪖 Helmet
* 🧤 Gloves
* 🦺 PPE / Safety Vest
* 🥾 Safety Shoes

If required PPE is missing, the system will identify the safety violation, trigger an alarm for a configurable duration, capture evidence, and record the violation for monitoring.

### 🚀 Development Roadmap

```text
Phase 1 → Environment Setup ✅
Phase 2 → Camera + OpenCV
Phase 3 → YOLO Person Detection
Phase 4 → PPE Detection
Phase 5 → Worker/PPE Association
Phase 6 → Safety Rules Engine
Phase 7 → Alarm System
Phase 8 → Violation Recording
Phase 9 → Dashboard
Phase 10 → Docker
Phase 11 → AWS Cloud
Phase 12 → Terraform
Phase 13 → GitHub Actions CI/CD
```

### 📌 Today's Progress

**Phase 1 completed successfully.**

Next: **Phase 2 → Camera integration and real-time video processing with OpenCV.**

Building this step by step with a focus on **AI + Computer Vision + Cloud + DevOps**.





.\venv\Scripts\python.exe -c "from ultralytics import YOLO; m=YOLO('yolo26n.pt'); m.train(data='data.yaml', epochs=1, imgsz=640, batch=4, device='cpu')"
