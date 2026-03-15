# 🛡️ **RetailGuard AI — Real-Time Civic Theft Detection**

**Behavioral AI • Pose-Based Monitoring • Community Protection • Open Source**
**YOLOv8 • XGBoost • Streamlit • Computer Vision**

<div align="center">
  <img src="https://img.shields.io/badge/AI-YOLOv8%20Pose-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Detection-Behavior%20Based-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Dashboard-Real--Time-success?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Backend-ML%20Pipeline-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" />
</div>

---

## 📚 Table of Contents

* [Overview](#overview)
* [The Civic Problem](#the-civic-problem)
* [Core Experience](#core-experience)
* [Detection Pipeline](#detection-pipeline)
* [System Architecture](#system-architecture)
* [Folder Structure](#folder-structure)
* [Tech Stack](#tech-stack)
* [Running Locally](#running-locally)
* [Deployment](#deployment)
* [Ethical Design](#ethical-design)
* [Why RetailGuard AI?](#why-retailguard-ai)

---

## 🌍 Overview

RetailGuard AI is an open-source, civic-focused retail security system designed to help small businesses detect suspicious shoplifting behavior using real-time computer vision.

It does not identify people.

It analyzes **behavioral patterns**.

Using pose estimation and machine learning, the system detects unusual body movements and logs suspicious activity to a monitoring dashboard.

Built to be:

* Affordable
* Transparent
* Deployable on standard hardware
* Open for community improvement

---

## 🏪 The Civic Problem

Retail theft disproportionately impacts small and community-owned businesses.

Enterprise surveillance systems are:

* Expensive
* Closed-source
* Designed for large corporations

RetailGuard AI provides:

* An open alternative
* Behavior-based detection
* Transparent ML logic
* Deployable without enterprise infrastructure

This is not corporate AI.
This is civic AI.

---

## 🎯 Core Experience

1. User uploads video or connects live feed
2. System detects human pose using YOLOv8
3. Behavioral features are extracted
4. ML classifier predicts suspicious vs normal
5. Dashboard logs incidents in real time
6. Alerts are stored for review

The system operates continuously and independently.

---

## 🧠 Detection Pipeline

### 🧍 1. Pose Estimation

* YOLOv8 Pose detects key body joints
* Extracts spatial coordinates of human posture
* Runs frame-by-frame analysis

### 📊 2. Feature Extraction

* Joint angles
* Body alignment
* Sudden motion changes
* Hand-object interaction patterns

### 🤖 3. Behavioral Classification

* XGBoost classifier
* Binary classification:

  * Suspicious
  * Normal
* Trained on extracted pose-based dataset

### 📋 4. Incident Logging

* Real-time dashboard
* Event summaries
* Stored suspicious timestamps
* Alert visualization

---

## 🏗️ System Architecture



<img width="1536" height="1024" alt="ChatGPT Image Mar 3, 2026, 06_02_33 AM" src="https://github.com/user-attachments/assets/bd2f7cc3-b789-408e-a8f0-4bf942ee881e" />







### Flow:

```
Video Input
    ↓
YOLOv8 Pose Estimation
    ↓
Feature Engineering
    ↓
XGBoost Classifier
    ↓
Real-Time Dashboard + Incident Log
```

The system separates:

* Vision detection
* Feature computation
* ML decision logic
* Visualization layer

Modular and extensible.

---

## 📁 Folder Structure

```text
RetailGuard-AI/
├─ README.md
│
├─ dashboardfinal.py
│   ├─ Streamlit UI
│   ├─ Video upload handling
│   ├─ Real-time alert rendering
│   └─ Incident logging interface
│
├─ model.py
│   ├─ Feature extraction logic
│   ├─ XGBoost loading
│   └─ Prediction pipeline
│
├─ trained_model.json
│   └─ Trained XGBoost model
│
├─ requirements.txt
│
└─ assets/
    ├─ alert sounds
    └─ sample test video
```

---

## 🧪 Tech Stack

### Computer Vision

* YOLOv8 Pose (Ultralytics)
* OpenCV (Headless)

### Machine Learning

* XGBoost
* Scikit-learn
* NumPy
* Pandas

### Interface

* Streamlit (real-time dashboard)

### Deployment

* Streamlit Cloud / Render

---

## ▶ Running Locally

```bash
git clone https://github.com/your-username/RetailGuard-AI.git
cd RetailGuard-AI

python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

pip install -r requirements.txt
streamlit run dashboardfinal.py
```

Open:

```
http://localhost:8501
```

---

## 🌐 Deployment

### Recommended

Deploy on:

* Streamlit Community Cloud
* Render (optional full-stack hosting)

Ensure:

* runtime.txt → python-3.11
* opencv-python-headless
* CPU-compatible torch

---

## 🔐 Ethical Design

RetailGuard AI:

* Does NOT use facial recognition
* Does NOT store biometric identity
* Detects behavioral anomalies only
* Designed for privacy-conscious monitoring
* Fully open-source for transparency

The goal is protection — not surveillance profiling.

---

## 🎯 Use Cases

* Small retail shops
* Community stores
* Local markets
* Civic safety research
* Behavioral AI experimentation
* Hackathon social good projects

---

## 📸 Screenshots


## Dashboard




<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/4a6f0a15-75e5-422e-809e-c3a60e5a2adb" />















<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/db3070b5-b25a-4d2a-bf97-338c982b1b1c" />







## NORMAL BEHAVIOUR





<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/216843b1-e92f-445f-b6bd-63ab643461aa" />






## SUSPICIOUS BEHAVIOUR





<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/d632ea0d-d9ab-49e7-98df-f41c0d3c8af0" />





## ALERTS AND CAPTURED FRAMES 





<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/05209f8b-9fa0-4575-a0da-0c7c3175dd4b" />







---

## 💭 Why RetailGuard AI?

> “Protection should not be exclusive to corporations.”

RetailGuard AI explores what happens when:

* Behavioral AI is transparent
* Detection avoids identity profiling
* Small businesses gain access to intelligent tools

It is not about surveillance.

It is about community resilience.

---

<p align="center" style="font-size:18px; color:#2563eb;">
  <i><b>“Behavior speaks. We listen.”</b></i>
</p>

---

