# 🚗 Real-Time Drowsiness Detection System

A computer vision system that detects driver drowsiness in real-time using facial landmark analysis.

## How It Works

The system uses **MediaPipe FaceMesh** to track 6 key landmarks per eye and computes the **Eye Aspect Ratio (EAR)** — a geometric ratio that drops sharply when eyes close. Once prolonged eye closure is detected, an audio alert is triggered immediately.

```
EAR = (A + B) / (2 × C)
```
Where A, B are vertical distances and C is the horizontal distance between eye landmarks.

## Features

- Real-time eye tracking with 468 facial landmarks
- EAR-based drowsiness detection
- Instant audio alert on drowsiness
- Annotated video output

## Tech Stack

- Python
- OpenCV
- MediaPipe
- NumPy

## Prerequisites
```bash
pip install opencv-python mediapipe numpy
```

