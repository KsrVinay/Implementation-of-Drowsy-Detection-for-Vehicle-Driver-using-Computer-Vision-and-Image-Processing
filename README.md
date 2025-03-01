## Overview  
This project is a **Drowsiness Detection System** that uses **computer vision and image processing** to detect driver fatigue in real-time. The system monitors **eye aspect ratio (EAR)** to determine if the driver is drowsy and triggers an alarm while increasing the system volume.

## Features  
- 🟢 Real-time **face and eye detection** using OpenCV & dlib  
- 🟢 Eye Aspect Ratio (EAR) calculation to detect drowsiness  
- 🟢 **Audio alert system** using pygame  
- 🟢 **Automatic volume control** using pycaw  
- 🟢 Works with a **webcam** for continuous monitoring  

## Installation  

### Prerequisites  
Ensure you have **Python 3.x** installed. Install the required dependencies

## How It Works
🔹 Face & Eye Detection
Detects facial landmarks using dlib’s shape predictor
Extracts eye regions from the face
🔹 Eye Aspect Ratio (EAR) Calculation
Computes the distance between key eye landmarks
If EAR falls below a threshold (0.25), drowsiness is detected
🔹 Drowsiness Alert Mechanism
If eyes remain closed for >3 seconds, alarm plays
System volume is increased to max
Volume is restored once the driver opens their eyes
Files
File	Description
drowsiness_detection.py	Main Python script for running the detection system
shape_predictor_68_face_landmarks.dat	Pre-trained model for detecting facial landmarks
beep11.mp3	Audio file for alert sound

## System Requirements
Hardware
🖥️ Webcam (for video input)
🔊 Speakers/Headphones (for alerts)
Software
🖥️ Operating System: Windows/Linux
🐍 Programming Language: Python 3.x
Future Enhancements
🚀 Integrate Deep Learning for better accuracy
📱 Develop a Mobile App for real-time monitoring
🌐 Cloud-based Monitoring for fleet management
