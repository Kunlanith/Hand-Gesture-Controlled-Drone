# Hand Gesture-Controlled Tello Drone

## Overview
This project enables users to control a **Tello drone** using **hand gestures**. By leveraging the **Mediapipe** library for real-time hand tracking and the **djitellopy** library for drone control, the system interprets hand movements captured by a webcam to execute specific drone actions. The drone responds to gestures such as landing, taking off, and moving in different directions based on the fold status of fingers and the position of the thumb.

## Features
- **Hand Gesture Recognition**: Uses Mediapipe for hand landmark detection and gesture recognition.
- **Real-Time Drone Control**: Commands sent to the Tello drone based on gestures.
- **Real-Time Feedback**: Displays hand landmarks and drone actions live on the screen.
  
## How It Works
1. **Hand Gesture Detection**: The system captures video feed via a webcam and processes it using Mediapipe to track hand landmarks.
2. **Gesture Analysis**: The program analyzes the fold status of each finger and the position of the thumb to identify specific gestures.
   - Example: All fingers folded and the thumb positioned left triggers the **land** command.
3. **Drone Control**: Based on the identified gesture, the corresponding drone action is executed using the djitellopy library.

## Video Demonstration
[![Hand Gesture-Controlled Tello Drone](https://img.youtube.com/vi/OblsApEg2zE/0.jpg)](https://youtu.be/OblsApEg2zE?si=D30BxCn2xKAKC2V7)

## Team Members
- **Akesit Akkharasaksir**  
- **Kunlanith Busabong**  
- **Pann Panyajaray**  
- **Paveetida Tiranatwittayakul**  
- **Rattapol Kitirak**  
- **Saranya Vichakyotin**  

## Requirements
- **Python Libraries**:
  - Mediapipe
  - djitellopy
  - OpenCV
  - NumPy
- **Hardware**:
  - Webcam for capturing hand gestures.
  - Tello drone.

## Installation

1. Install required libraries:
   ```bash
   pip install mediapipe djitellopy opencv-python numpy
   ```

2. Set up your webcam and Tello drone.

3. Run the script to start controlling the drone with hand gestures.

## Results
- The drone successfully responds to hand gestures in real-time, performing actions like **takeoff**, **land**, and **movement** based on specific gestures.

## Future Work
- **Gesture Expansion**: Add more complex gestures for additional control options (e.g., yaw, roll, pitch).
- **Enhanced Stability**: Improve gesture recognition accuracy for smoother drone control.
