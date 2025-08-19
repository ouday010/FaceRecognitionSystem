# FaceRecognitionSystem

A simple Python-based face recognition system. Collects face images from a webcam, trains a CNN model to recognize multiple people, and performs real-time face identification using OpenCV and TensorFlow.

---

## Features

- Captures face images with OpenCV’s Haar Cascade.
- Trains a multi-class CNN model for face recognition.
- Recognizes faces in real-time with confidence scores.
- Easy to use for personal projects.

---

## Prerequisites

- Python 3.6+
- Webcam
- Basic command-line knowledge

---

## Installation

**Clone the repository:**
```bash
git clone https://github.com/ouday010/FaceRecognitionSystem.git
cd FaceRecognitionSystem
```

**Install dependencies:**
```bash
pip install opencv-python tensorflow numpy
```

**Verify Haar Cascade:**
- `haarcascade_frontalface_default.xml` is included with opencv-python.
- If missing, download it from OpenCV’s GitHub.

---

## Usage

### 1. Collect Face Images

Run to capture face images:
```bash
python FaceImageCollector.py
```
- Enter a name (e.g., “john”).
- Saves up to 500 images to `images/john/`.
- Press 'q' to stop early.
- Repeat for each person.

---

### 2. Train the Model

Run to train the model:
```bash
python FaceModelTrainer.py
```
- Uses images in `images/` (e.g., `images/john`, `images/jane`).
- Saves `face_recognition_model.h5` and `class_indices.json`.

---

### 3. Real-Time Recognition

Run to recognize faces:
```bash
python FaceRecognizer.py
```
- Opens webcam, shows names (e.g., “john (0.95)”) on detected faces.
- Press 'q' to stop.
