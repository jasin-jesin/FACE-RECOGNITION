# Face Recognition — Python

> Python | OpenCV | Haar Cascade | Face Detection & Recognition

## Overview

A Python-based face recognition system that includes the full pipeline: capturing headshots, training a model, detecting faces, and recognising individuals. Built using OpenCV and classical machine learning techniques.

## Project Structure

| File | Description |
|---|---|
| headshots.py | Captures face images from webcam for training data |
| train_model.py | Trains the face recognition model from captured images |
| face_ditect.py | Real-time face detection using Haar Cascade classifier |
| facial_req.py | Face recognition — matches detected faces to known identities |
| haarcascade_frontalface_default.xml | Pre-trained Haar Cascade model for face detection |

## How It Works

1. **Capture** — Run headshots.py to collect face images from your webcam
2. **Train** — Run train_model.py to build a recognition model from the images
3. **Detect** — Run face_ditect.py to detect faces in real time
4. **Recognise** — Run facial_req.py to identify faces against the trained model

## Requirements

pip install opencv-python numpy

## Usage

### Step 1 — Capture training images
python headshots.py

### Step 2 — Train the model
python train_model.py

### Step 3 — Run face recognition
python facial_req.py

## Features

- Webcam-based face capture for building a training dataset
- Model training with LBPH (Local Binary Pattern Histogram) or similar
- Real-time face detection using Haar Cascade
- Identity recognition with confidence scoring
- Saved model for reuse without retraining

## Notes

- Works best with good lighting and a front-facing camera
- Add more training images per person to improve accuracy
