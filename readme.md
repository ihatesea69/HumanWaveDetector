# HumanWaveDetector

<video src="https://github.com/user-attachments/assets/d7868488-5968-4b2c-b7df-4da830d4f4d2" controls autoplay muted loop></video>

A real-time computer vision application using MediaPipe and OpenCV to detect human hand gestures and body pose. Displays "Hello" greeting when a waving hand gesture is recognized through the webcam.

## Table of Contents

1. [Overview](#overview)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Customization](#customization)
6. [Contact](#contact)

## Overview

HumanWaveDetector is a Python application that uses your webcam to detect hand gestures and body poses in real-time. When a person waves their hand at the camera, the application recognizes the gesture and prints a greeting message.

### Key Features

- Real-time hand detection and tracking using MediaPipe Hands
- Body pose detection using MediaPipe Pose
- Visual overlays showing detected hand landmarks and body skeleton
- Automatic wave gesture recognition
- Optimized frame processing for smooth performance

## Prerequisites

- Python >= 3.7
- Webcam

## Installation

### Clone Repository

```bash
git clone https://github.com/ihatesea69/HumanWaveDetector.git
cd HumanWaveDetector
```

### Install Dependencies

```bash
pip install opencv-python mediapipe
```

Or install via setup.py:

```bash
python setup.py install
```

## Usage

Run the application:

```bash
python main.py
```

### Controls

- Press `q` to quit the application

### How It Works

1. The application captures video from your webcam
2. Each frame is processed to detect hands and body pose
3. When a waving gesture is detected (thumb and index finger in specific positions), "Xin Chào Bạn" (Hello) is printed
4. Visual overlays show the detected landmarks on the video feed

## Customization

Modify the wave detection logic in `main.py` to adjust gesture recognition:

```python
if landmarks[4].x > landmarks[3].x and landmarks[8].y < landmarks[6].y:
    waving_hand = True
```

## Contact

For questions or issues, contact via [Facebook](https://www.facebook.com/danhhoanghieunghi69/).

---

**HUFLIT Student Project**
