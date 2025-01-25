# Volume-control-using-Hand

This repository contains a Python script that uses a webcam to control the system volume based on hand gestures. The script employs the MediaPipe library to detect hand landmarks and PyAutoGUI to adjust the volume.

# Features

Real-time hand tracking using MediaPipe.
Volume control by detecting the distance between the index finger and thumb.
Visual feedback using OpenCV to display the hand landmarks and gestures.

# Requirements

Before running the script, make sure you have the following dependencies installed:
Python 3.6+
OpenCV (cv2)
MediaPipe
PyAutoGUI

# Code Overview

Setup:
The webcam is initialized using OpenCV.
MediaPipe's Hands module is used for detecting and tracking hand landmarks.

Processing Frames:
Each frame is captured, flipped, and converted to RGB format.
Hand landmarks are detected and drawn on the frame.

Volume Control:
The script calculates the distance between the tip of the thumb and the index finger.
If the distance exceeds a threshold, the volume is increased; otherwise, it is decreased.

Display and Exit:
The processed frame is displayed in a window.
Press the Esc key to exit the application.

# Notes

Ensure that your webcam is functioning properly.
The script uses PyAutoGUI to control the volume; make sure you have the necessary permissions for automation.
Adjust the distance threshold (dist > 50) in the script if the gestures do not map well to volume changes.

# Example Output

A window will display the live webcam feed with hand landmarks drawn.
The distance between the index finger and thumb will be visualized with a line.
Volume changes will occur in real-time based on the gesture.
