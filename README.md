# 🛍️ Shoplifting Detection using YOLO Pose Estimation

> **An intelligent surveillance system** that detects shoplifting behavior using **YOLOv8 Pose Estimation** and **XGBoost Classification**.  
> Real-time detection of suspicious movements through human pose analysis — bringing AI vision to retail security.

---     

<div align="center">

| 🧠 **AI Model** | ⚙️ **Core Tech** | 🎯 **Domain** | 🚀 **Status** |
|:---------------:|:----------------:|:-------------:|:-------------:|
| YOLOv8-Pose + XGBoost | OpenCV, Pandas, NumPy | Smart Surveillance | ✅ Active Development |

</div>

---

## 🧭 Table of Contents

- [🎥 Demo](#-demo)
- [💡 Project Overview](#-project-overview)
- [⚙️ How It Works](#️-how-it-works)
- [🖼️ Features](#️-features)
- [🧩 Requirements](#-requirements)
- [🚀 Installation](#-installation)
- [▶️ Usage](#️-usage)
- [📁 Project Structure](#-project-structure)
- [🧠 Why This Project](#-why-this-project)
- [📜 License](#-license)
- [🤝 Contributing](#-contributing)

---

## 🎥 Demo

> 🎬 **[Watch the Demo Video]*  
*(Replace this link with your actual Google Drive demo video link — use “Anyone with link → Viewer” setting.)*

---

## 💡 Project Overview

This project implements a **shoplifting detection system** that monitors surveillance video in real-time.  
Using **YOLOv8 Pose Estimation**, it captures human joint positions, and through **XGBoost classification**, it identifies abnormal or suspicious behavior.

It merges **computer vision** and **machine learning** to provide a cost-effective, scalable, and intelligent store security solution.

> “We didn’t just detect movement — we taught machines to understand human intent.”

---

## ⚙️ How It Works

1. **Pose Detection:**  
   YOLOv8 extracts skeletal keypoints (body joints) from live video frames.

2. **Feature Extraction:**  
   These keypoints are converted into feature vectors representing human posture and motion.

3. **Behavior Classification:**  
   An XGBoost model classifies the detected action as **Normal** or **Suspicious**.

4. **Real-Time Output:**  
   OpenCV displays live bounding boxes, labels, and confidence levels on the video feed.

---

## 🖼️ Features

✅ Real-time human pose detection using YOLOv8  
✅ Behavior classification with XGBoost  
✅ Works with webcam or recorded video  
✅ Interactive visualization using OpenCV  
✅ Custom dataset creation and retraining supported  
✅ Scalable for multi-camera surveillance systems  

---

## 🧩 Requirements

```bash
Python 3.11+
OpenCV
Ultralytics YOLO
XGBoost
Pandas
NumPy
cvzone

Installation

Clone the repository

git clone [your-repo-url]
cd [repo-name]


Create and activate a virtual environment

python -m venv venv
# Windows
.\venv\Scripts\activate
# Linux/Mac
source venv/bin/activate


Install dependencies

pip install -r requirements.txt

▶️ Usage

Create Dataset

python datset.py


Collect normal and suspicious pose data from video frames.

Train Model

python model.py


Train an XGBoost classifier using the extracted dataset.

Run Real-Time Detection

python main.py


Launches live detection and visualization.
Press ‘q’ to quit the application.

📁 Project Structure
shoplifting-detection-yolo/
├── main.py               # Main application for real-time detection
├── dataset.py            # Dataset creation and preprocessing
├── model.py              # XGBoost model training
├── Normal.py             # Normal behavior data collection
├── Suspicious.py         # Suspicious behavior data collection
├── requirements.txt      # Dependencies
└── README.md             # Documentation

🧠 Why This Project

Retail theft leads to billions in global losses every year.
This project aims to provide a non-invasive, AI-based surveillance system that helps detect suspicious actions automatically and assist human security operators.

Goal: To make retail spaces safer using ethical and intelligent AI vision.


🤝 Contributing

Contributions are always welcome!
If you’d like to improve detection accuracy, optimize models, or enhance visualization — please open an issue or submit a pull request.

Built with Intelligence. Secured with Vision.


Testing SSH verified commit

Testing verified commit final