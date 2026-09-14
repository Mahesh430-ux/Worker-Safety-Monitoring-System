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




Day 3:- 
Added 4 new slides
Today's Project Work → GitHub
PPE/safety detection model training
Flask/backend debugging
Dependency checking
GitHub Version of Today's Work
git status
git add
git commit
git pull
git push
Recommended GitHub Project Structure
camera/
routes/
models/
templates/
static/
requirements.txt
README.md
.gitignore
README: Show What You Built Today
Today's progress
Tech stack
Next steps





# 🚀 Day 4: AI Model Training & Safety Detection Integration

Today, I focused on integrating the trained AI model into the **AI-Based Worker Safety Monitoring System** and preparing the project for real-time safety monitoring.

## 🔹 Work Completed Today

### 1. 🤖 Trained the YOLO Object Detection Model

* Trained a custom YOLO model using the prepared worker-safety dataset.
* The model was trained to identify safety-related conditions from camera images.
* Verified that the training process completed successfully.
* Training results and model weights were generated successfully.

### 2. 🦺 Safety Gear Detection

The AI system is designed to detect whether workers are following required safety protocols, including:

* ⛑️ Helmet / No Helmet
* 🦺 Safety Vest / No Safety Vest
* 👷 Worker detection
* ⚠️ Safety violations

The detection system can analyze camera frames and identify potential PPE violations.

### 3. 🚨 Automatic Safety Alarm Concept

Implemented the logic required for an automatic alert mechanism.

When the AI detects a critical safety violation such as:

> **Worker detected without a helmet**

the system can trigger an automatic **siren/alarm notification**.

This creates a real-time safety response mechanism instead of only displaying the violation on the dashboard.

### 4. 📊 Admin Dashboard Integration Preparation

Prepared the AI detection output for integration with the project's professional admin dashboard.

The dashboard is planned to display:

* 📹 Live camera feed
* 👷 Number of workers detected
* ⛑️ Helmet compliance
* 🦺 Safety-vest compliance
* ⚠️ Active violations
* 🚨 Alarm status
* 📸 Detection evidence
* 📈 Safety statistics
* 🕒 Recent safety events

### 5. 🧠 Detection → Alert Workflow

The planned system workflow is:

```text
Camera
   ↓
Video/Image Frame
   ↓
YOLO AI Model
   ↓
Worker & PPE Detection
   ↓
Safety Rule Verification
   ↓
 ┌─────────────────────┐
 │ Safety Compliant?   │
 └─────────┬───────────┘
           │
      ┌────┴────┐
      │         │
     YES        NO
      │         │
      ↓         ↓
 Dashboard   Violation
 Update         ↓
             Alarm
               ↓
        Admin Notification
               ↓
        Evidence Storage
```

## 🛠️ Technologies Used

* **Python**
* **YOLO / Ultralytics**
* **OpenCV**
* **Flask**
* **HTML**
* **CSS**
* **JavaScript**
* **NumPy**
* **Computer Vision**
* **Machine Learning**

## 📂 Project Progress

```text
Day 1  → Project planning & problem analysis        ✅
Day 2  → Dataset preparation & preprocessing        ✅
Day 3  → YOLO model setup & training                ✅
Day 4  → Model verification & safety integration    ✅
Day 5  → Dashboard & real-time camera integration   🔄
```

## 🎯 Day 4 Outcome

The major achievement of Day 4 was successfully moving the project from **AI model training toward real-time safety monitoring**.

The trained model is now ready to become the core detection engine of the system.

### 🔥 Next Step — Day 5

Next, I will focus on:

* Building the professional **3D Admin Dashboard**
* Connecting the YOLO model with the Flask backend
* Adding real-time camera detection
* Displaying PPE violations on the dashboard
* Implementing automatic siren activation
* Saving violation evidence
* Adding safety statistics and monitoring features

---

### 💡 Project Vision

> **"Detect the risk before it becomes an accident."**

This project aims to create an intelligent industrial safety monitoring system capable of continuously monitoring workers, detecting PPE violations, generating alerts, and providing administrators with real-time safety information.
