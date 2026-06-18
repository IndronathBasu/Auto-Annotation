# 🚀 AutoAnnotate AI

> Intelligent Offline Auto Annotation Platform for Computer Vision Datasets

AutoAnnotate AI is a desktop-based annotation tool that combines manual labeling, AI-assisted propagation, YOLO training, human review workflows, and dataset balancing analytics into a single application.

The goal is to dramatically reduce the time required to create high-quality object detection datasets while maintaining annotation accuracy.

---

# ✨ Features

## 🎯 Manual Annotation

* Click-and-drag bounding box annotation
* Multi-class support
* Add, rename, and remove classes
* Fast image navigation
* Annotation editing and deletion

---

## 🤖 AI-Assisted Annotation

Train a YOLO model on a small subset of manually annotated images and automatically propagate labels to the remaining dataset.

### Workflow

1. Add Classes
2. Annotate 10–20 Images
3. Train YOLO
4. Propagate Labels
5. Review Predictions
6. Export Dataset

This can reduce annotation effort by up to **90%**.

---

## 👨‍💻 Human Review System

Low-confidence predictions are automatically separated for review.

Features:

* Adjustable confidence threshold
* Accept predictions
* Reject predictions
* Edit labels
* Quality assurance workflow

---

## 📊 Dataset Balance Monitor

Built-in dataset balancing analytics help maintain a healthy training dataset.

### Recommended Target

> Minimum 30 samples per class

### Color Coding

| Status  | Count |
| ------- | ----- |
| 🔴 LOW  | < 20  |
| 🟡 FAIR | 20–29 |
| 🟢 GOOD | ≥ 30  |

Example:

```text
Nut_SV     18   🔴 Need 12 More
Nut_TV     27   🟡 Need 3 More
Bolt_A     35   🟢 Ready
```

---

## 🏋️ Custom YOLO Training

Supported Models:

* YOLOv8n
* YOLOv8s
* YOLOv8m
* YOLOv8l
* YOLOv8x
* Segmentation Models

Features:

* GPU Acceleration
* Adjustable Epochs
* Automatic Dataset Generation
* Offline Training

---

## 🎬 Video Support

Convert videos into training datasets.

Supported Features:

* Open video files
* Select extraction FPS
* Generate training frames
* Annotate extracted images

---

## 💾 Persistent Project Saving

Automatically stores:

* Annotations
* File Lists
* Classes
* Model Configuration
* Current Progress

Resume your work anytime.

---

# 🏗️ System Architecture

```text
Images / Video
       │
       ▼
Manual Annotation
       │
       ▼
YOLO Dataset Creation
       │
       ▼
Custom Model Training
       │
       ▼
AI Propagation
       │
       ▼
Human Review
       │
       ▼
Dataset Balancing
       │
       ▼
Export YOLO Dataset
```

---

# 📂 Supported Formats

### Images

* JPG
* JPEG
* PNG
* BMP
* TIFF
* WEBP

### Labels

* YOLO TXT Format

### Models

* YOLOv8 Detection
* YOLOv8 Segmentation

---

# 🛠️ Technology Stack

## Frontend

* CustomTkinter
* Tkinter
* Pillow

## Computer Vision

* OpenCV

## Deep Learning

* Ultralytics YOLO
* PyTorch

## Utilities

* NumPy
* Threading
* JSON Configuration Storage

---

# 📦 Installation

## Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/AutoAnnotateAI.git
cd AutoAnnotateAI
```

## Create Virtual Environment

```bash
python -m venv venv
```

## Activate Virtual Environment

### Windows

```bash
venv\Scripts\activate
```

### Linux / Mac

```bash
source venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Application

```bash
python main.py
```

---

# 📁 Project Structure

```text
AutoAnnotateAI/
│
├── main.py
├── requirements.txt
├── .gitignore
│
├── models/
│   ├── yolov8m.pt
│   └── yolo26n.pt
│
├── runs/
│
├── datasets/
│
└── venv/
```

---

# ⚙️ Recommended Hardware

## Minimum

* Intel i5
* 8 GB RAM
* Integrated Graphics

## Recommended

* Intel i7 / Ryzen 7
* 16 GB RAM
* NVIDIA GPU with CUDA Support
* SSD Storage

---

# 🏭 Industrial Applications

## Manufacturing

* Bolt Detection
* Nut Detection
* Tool Detection
* Assembly Verification

## Automotive

* Engine Assembly Inspection
* Fastener Tracking
* Quality Control

## Healthcare

* Medical Image Annotation
* Disease Localization

## Agriculture

* Crop Monitoring
* Fruit Detection

## Retail

* Product Detection
* Shelf Analytics

---

# 📈 Future Roadmap

* Polygon Annotation
* Instance Segmentation
* Active Learning
* Automatic Data Augmentation
* Multi-User Collaboration
* ONNX Export
* TensorRT Export
* Cloud Synchronization

---

# 🎯 Advantages

* Fully Offline
* No Subscription Required
* GPU Accelerated
* Human-in-the-Loop Review
* Dataset Balance Monitoring
* Integrated YOLO Training
* Production-Ready Dataset Export

---

# 📄 License

MIT License

---

# 👨‍💻 Author

Developed to accelerate industrial-scale computer vision dataset creation through intelligent AI-assisted annotation workflows.
