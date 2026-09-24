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


🚧 Worker Safety Monitoring System — Day 5
📅 Day 5 Progress

Today I focused on improving the PPE verification architecture and planning the system for deployment across multiple construction-site zones.

✅ Work Completed
Designed a false-alarm elimination strategy for PPE detection.
Planned systematic testing for:
Helmet / No Helmet
Vest / No Vest
Gloves / No Gloves
Goggles / No Goggles
Boots / No Boots
Planned testing under:
Different lighting conditions
Different camera angles
Multiple workers
Different helmet colors
Partially blocked workers
Designed a 4-zone monitoring architecture.
Decided to use one centralized database instead of separate databases for each zone.
Planned zone-specific PPE requirements using a Safety Rule Engine.
Separated AI detection from zone safety rules.
Planned temporal verification so that a single incorrect frame does not immediately trigger the alarm.
Planned future support for IP/RTSP construction-site cameras instead of relying only on the laptop webcam.
Designed the future workflow:
Camera
   ↓
Person Detection
   ↓
PPE Detection
   ↓
Zone Detection
   ↓
Zone PPE Rules
   ↓
Temporal Verification
   ↓
Safety Decision
   ↓
Database + Dashboard + Alarm
🧪 Planned Testing Strategy

The PPE model will be tested in phases:

Phase 1: Basic PPE verification
Phase 2: False-positive testing
Phase 3: Lighting & camera-angle testing
Phase 4: Multiple-worker testing
Phase 5: Four-zone safety-rule implementation
Phase 6: Live construction-site camera integration

🏗️ Planned Zones

The system architecture will support four different site zones, for example:

Zone 1 → Chemical Zone
Zone 2 → Construction Zone
Zone 3 → Specialized Zone
Zone 4 → General Zone

Each zone can have its own required PPE configuration.

💡 Key Design Decision

Instead of creating a separate AI model/database for every zone:

One AI model + One centralized database + Zone-specific safety rules

This makes the system easier to maintain and allows the admin to modify PPE requirements without retraining the entire model.

🚀 Next Steps — Day 6

Tomorrow I will start with Phase 1: PPE Verification & False Alarm Testing.

The first goal will be to test the current YOLO model systematically and identify where false detections occur before implementing the four-zone system.




# Day 6 — PPE Dataset Cleaning & Visual Annotation Audit

## 📅 Progress Update

Today I focused on improving the quality and reliability of the PPE detection dataset before starting the next YOLO training cycle.

The goal was to reduce incorrect annotations and improve the model's ability to distinguish between compliant and non-compliant safety equipment.

---

## 🔍 1. Dataset Structure Validation

The complete PPE dataset was inspected across:

- Training dataset
- Validation dataset
- Testing dataset

Total label files checked:

**5,140**

Total annotations:

**21,584**

Dataset structure verification confirmed:

- No malformed annotation files
- No empty label files
- No images without labels
- No labels without corresponding images

The dataset structure and YOLO annotation format are now valid.

---

## 🛠️ 2. Segmentation Annotation Cleanup

During the initial annotation validation, 54 polygon/segmentation annotations were identified.

These annotations were converted into YOLO detection-format bounding boxes.

Conversion result:

- Normal detection annotations retained: 21,531
- Polygon annotations converted: 54
- Conversion errors: 0

All identified polygon annotations were successfully converted.

---

## 👷 3. PPE Class Distribution Audit

The dataset currently contains 10 PPE-related classes:

| ID | Class | Annotations |
|---:|---|---:|
| 0 | boots | 4,601 |
| 1 | gloves | 1,549 |
| 2 | goggles | 588 |
| 3 | helmet | 5,892 |
| 4 | no-boots | 163 |
| 5 | no-gloves | 334 |
| 6 | no-goggles | 843 |
| 7 | no-helmet | 598 |
| 8 | no-vest | 1,175 |
| 9 | vest | 5,841 |

This audit also revealed that some violation classes have significantly fewer samples than their corresponding compliant classes.

---

## 🪖 4. Helmet Annotation Visual Audit

A visual audit was performed for helmet annotations.

The audit identified suspiciously large helmet bounding boxes for manual inspection.

Instead of automatically deleting these annotations, preview images were generated so that each annotation could be visually verified.

This helped distinguish between:

- Correct large bounding boxes
- Incorrect bounding boxes
- Objects occupying a large portion of the image
- Possible annotation mistakes

The audit showed that bounding-box size alone should not be used to remove an annotation.

---

## 🚨 5. No-Helmet Dataset Audit

The `no-helmet` class was specifically audited.

Total:

**598 no-helmet annotations**

Visual inspection was started to verify whether the bounding boxes correctly represented workers without helmets.

This is particularly important because `no-helmet` is one of the critical classes responsible for triggering the safety alarm.

---

## 🦺 6. No-Vest Dataset Audit

The `no-vest` class was also audited.

Total:

**1,175 no-vest annotations**

A suspicious-box scan identified:

**131 potentially large no-vest bounding boxes**

These were not automatically deleted.

Instead, visual audit previews were generated for manual verification.

Initial inspection showed that large boxes can still represent valid no-vest annotations when the worker occupies a large portion of the image.

---

## 🧠 7. False-Positive Prevention Strategy

A major focus of today's work was preventing the AI system from triggering alarms because of incorrect training annotations.

The planned pipeline is:


Dataset
   ↓
Annotation Validation
   ↓
Visual Audit
   ↓
Dataset Strengthening
   ↓
YOLO Training
   ↓
Validation
   ↓
Real Camera Testing
   ↓
False-Positive Testing
   ↓
Alarm Trigger





Day 7 — Dataset Strengthening & Custom Zone Configuration
📅 Progress Update

Today, the Worker Safety Monitoring System was advanced from basic dataset preparation toward zone-aware safety monitoring.

✅ Work Completed Today
1. Added External Construction PPE Dataset

Integrated the Ultralytics Construction-PPE dataset as an external dataset for strengthening the existing PPE detection dataset.

The dataset contains classes such as:

Helmet
Gloves
Vest
Boots
Goggles
No Helmet
No Gloves
No Goggles
No Boots
Person
None

The external dataset was kept separate initially to avoid damaging the original dataset.

2. External Dataset Conversion

Created a conversion pipeline to map the external dataset classes into the project's existing 10-class structure.

Project classes
0  boots
1  gloves
2  goggles
3  helmet
4  no-boots
5  no-gloves
6  no-goggles
7  no-helmet
8  no-vest
9  vest

The conversion successfully processed the external annotations.

Conversion result
Label files processed : 1426
Images selected       : 1414
Images skipped        : 10
Annotations converted : 8479

The converted dataset was then prepared for integration.

3. Dataset Strengthening

Created a separate strengthening workspace:

Downloads/
└── strengthening/
    ├── construction_ppe_external/
    ├── audit/
    ├── preview/
    ├── selected/
    └── combined_dataset/

This approach keeps the original dataset protected while allowing additional verified data to be introduced.

4. Visual Annotation Verification

Created preview images from the converted dataset and manually inspected the annotations.

The PPE bounding boxes were visually checked and confirmed to be usable for training.

5. Weak-Class Audit

Audited the important PPE classes, particularly:

no-helmet
no-gloves
no-boots
no-goggles
goggles

The purpose was to identify whether the additional dataset would improve the weaker classes and reduce false positives.

6. Combined Dataset Created

Successfully merged the original dataset with the verified converted external dataset.

Final combined dataset:

Train : 2260 images / 2260 labels
Valid : 286 images / 286 labels
Test  : 282 images / 282 labels

Total : 2828 images
Labels: 2828
Annotations: 16958
7. Dataset Validation

The final combined dataset passed validation.

✅ No missing image/label pairs
✅ No malformed annotations
✅ No invalid class IDs
✅ No invalid YOLO coordinates

This confirms that the combined dataset is structurally ready for the next training stage.

8. Four-Zone Safety Architecture

Configured the project's four required operational zones:

Camera 1
│
├── Zone A — Construction
├── Zone B — Chemical
├── Zone C — Electrical
└── Zone D — General

Configured PPE requirements:

Zone	Required PPE
Construction	Helmet, Vest, Boots
Chemical	Helmet, Vest, Gloves, Goggles, Boots
Electrical	Helmet, Vest, Gloves, Boots
General	Helmet, Vest, Boots

These are the current prototype rules and should ultimately be aligned with the actual site's safety policy.

9. Custom Polygon Zone Editor

Implemented and tested a custom polygon-based zone editor.

Created:

zones/
├── config.py
├── zone_detector.py
├── zone_editor.py
├── zones.json
└── __init__.py

The editor allows the user to click points on the camera image and define custom zone boundaries.

Successfully created and saved:

Zone A - Construction
Zone B - Chemical
Zone C - Electrical
Zone D - General

The saved configuration is:

zones/zones.json
10. Custom Zone Detector Tested

Verified that zone_detector.py successfully loads:

Zone A - Construction: 4 points
Zone B - Chemical: 4 points
Zone C - Electrical: 4 points
Zone D - General: 4 points

The custom polygon system is therefore functioning.

⚠️ Issue Identified Today

When the first polygons were created, they overlapped heavily.

This caused the dashboard to display zone names on top of each other.

The problem was identified as a zone-boundary configuration issue, not a YOLO detection issue.

A backup of the original zone configuration was created before correcting the boundaries.

The next configuration should use non-overlapping polygons so that a worker is assigned to one zone at a time.




# Day 8 — Zone-Based Worker Safety Detection & Intelligent Alarm

## Work Completed Today

Today, the Worker Safety Monitoring System was successfully extended from basic PPE detection to a zone-aware intelligent safety monitoring system.

### 1. Fixed Custom Zone Detection

Implemented and tested a custom four-zone architecture:

- Zone A — Construction
- Zone B — Chemical
- Zone C — Electrical
- Zone D — General

The system now correctly identifies the worker's zone using the worker bounding-box center.

### 2. Fixed Zone Detector

Updated:

zones/zone_detector.py

The zone detector now:

- Loads zones from zones.json
- Supports dictionary-based zone configuration
- Detects whether a worker is inside a zone
- Determines the worker's zone from the bounding-box center
- Draws zone boundaries and labels on the camera frame

### 3. Worker Detection

Integrated a person detector with the safety detection pipeline.

The system can now:

- Detect workers
- Assign Worker IDs
- Generate worker bounding boxes
- Determine the worker's current zone

Example:-
Worker 1
Zone D - General






# Day 9 — Smooth Camera Optimization & Gmail Safety Alerts

## Work Completed Today

Today, the Worker Safety Monitoring System was improved in two major areas:

1. Live camera performance optimization
2. Gmail safety notification integration

---

## 1. Smooth Live Camera Optimization

Previously, the camera was lagging because the AI detection pipeline was processing every camera frame.

### Problem

The AI processing time was approximately:

- AI processing: ~340 ms per frame
- Camera display: ~3–4 FPS

This caused noticeable camera lag and delayed movement.

Solution:- 
Implemented frame-skipping based AI processing.

Instead of running the AI model on every frame:-
Camera Frame 1 → Display
Camera Frame 2 → Display
Camera Frame 3 → AI Detection
Camera Frame 4 → Display
Camera Frame 5 → Display
Camera Frame 6 → AI Detection



System
📅 Day 9 Progress

Today, I focused on improving the real-time performance of the AI-based Worker Safety Monitoring System and developing the alert notification pipeline.

✅ Work Completed
Optimized the real-time camera processing for smoother video performance.
Implemented AI inference every 3 frames while displaying every camera frame.
Improved camera responsiveness and reduced the visual lag caused by continuous AI inference.
Tested the optimized camera with the YOLO-based safety detection system.
Integrated the Intelligent Alarm concept for confirmed PPE violations.
Implemented violation confirmation logic to reduce false alarms caused by temporary detection fluctuations.
Added configurable alarm confirmation frames and cooldown logic.
Integrated Gmail email notifications for safety violations.
Successfully tested Gmail SMTP integration and confirmed that safety alerts can be sent successfully.
Added notification handling for:
Zone information
Worker ID
Missing PPE
Violation details
Started integration of SMS notifications.
Tested Twilio SMS integration, but the trial account encountered restrictions.
Investigated alternative notification services for future SMS/phone alerts.
Kept sensitive credentials inside .env instead of committing them to GitHub.
Continued organizing the project into separate modules for detection, zones, alarms, and notifications.





## Day 10 – Notification System & Database Integration

Today, I completed the notification layer of the AI Worker Safety Monitoring System and started integrating MongoDB for centralized data storage.

### ✅ Completed

- Implemented Gmail safety violation notifications.
- Successfully tested Gmail alert delivery.
- Implemented Telegram Bot API notifications.
- Successfully tested Telegram alerts on mobile.
- Replaced the previous Twilio SMS approach with Telegram for the current prototype.
- Integrated Gmail and Telegram into the centralized notification manager.
- Added threaded notification execution to prevent blocking the main safety system.
- Added proper notification success/failure reporting.
- Continued development of the optimized smooth-camera pipeline.
- Continued intelligent alarm development with violation confirmation logic.
- Started MongoDB Atlas integration.
- Installed and configured PyMongo.
- Created MongoDB connection layer.
- Configured MongoDB environment variables using `.env`.
- Verified MongoDB Atlas DNS resolution.
- Verified connectivity to MongoDB Atlas on port 27017.
- Configured MongoDB Atlas IP access requirements.

### 🏗️ Current Architecture

Camera
↓
Person Detection
↓
Zone Detection
↓
PPE Detection
↓
Violation Confirmation
↓
Intelligent Alarm
├── 🔊 Safety Siren
├── 📧 Gmail Alert
└── 📱 Telegram Alert

MongoDB integration is currently being finalized for:

- Violation records
- Worker information
- Zone information
- Notification history
- Evidence-image metadata
- GridFS-based evidence storage

### 🔜 Next Steps

1. Complete MongoDB Atlas connection.
2. Test MongoDB database operations.
3. Implement GridFS.
4. Upload and retrieve a test evidence image.
5. Connect confirmed violations with MongoDB.
6. Store violation metadata and evidence references.
7. Build the dashboard database layer.
8. Evaluate cloud storage strategy for the training dataset.

### 🔐 Security

Sensitive credentials are stored in `.env` and are not committed to GitHub.

The project continues to follow a modular architecture separating:

- AI detection
- Zone management
- Safety rules
- Alarm management
- Notifications
- Database
- Dashboard





Day 11 – PPE Dataset Strengthening & Multi-Zone Safety Detection

Integrated the Ultralytics Construction-PPE dataset with the existing PPE dataset.
Converted and validated external YOLO annotations.
Created a combined PPE dataset containing 2,828 images and 16,958 annotations.
Verified image-label pairs and YOLO annotation validity.
Configured four safety zones:
Zone A – Construction
Zone B – Chemical
Zone C – Electrical
Zone D – General
Implemented custom polygon-based zone detection.
Improved worker-to-PPE association using bounding-box overlap and IoU.
Implemented zone-specific PPE requirements.
Tested the trained PPE model independently from the zone detection pipeline.
Investigated false PPE detections using raw model output.
Identified that current false positives originate from the trained PPE model and require further dataset/model investigation.

Current Status: Multi-zone detection pipeline is functional, while PPE model accuracy and false-positive reduction are the next development task.



Day 12 :- PPE Detection Investigation & Model Validation

Verified the trained YOLO model configuration.
Investigated false PPE detections from best.pt.
Tested the PPE model independently from the zone-processing pipeline.
Identified false detections such as face → helmet and T-shirt → vest.
Verified that the false detections originate from the trained PPE model rather than only the zone association logic.
Inspected the model training configuration.
Found that the train-5 model was trained for only 1 epoch.
Located multiple data.yaml files and began identifying the exact dataset used for train-5.
Paused retraining until the correct dataset and class mapping are verified.
