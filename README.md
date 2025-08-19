# FaceRecognitionSystem
FaceRecognitionSystem: A Python-based pipeline for face recognition. Collects face images with OpenCV, trains a CNN model using TensorFlow for multi-class identification, and performs real-time recognition. Simple, robust, and professional for personal or small-scale use. MIT licensed.


FeaturesCaptures face images with OpenCV’s Haar Cascade.
Trains a multi-class CNN model for face recognition.
Recognizes faces in real-time with confidence scores.
Easy to use for personal projects.

PrerequisitesPython 3.6+
Webcam
Basic command-line knowledge

InstallationClone the repository:bash

git clone https://github.com/your-username/FaceRecognitionSystem.git
cd FaceRecognitionSystem

Install dependencies:bash

pip install opencv-python tensorflow numpy

Verify Haar Cascade:haarcascade_frontalface_default.xml is included with opencv-python. If missing, download it from OpenCV’s GitHub.

