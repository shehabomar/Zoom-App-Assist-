# Student Focus Detection System

This project uses computer vision and text-to-speech capabilities to detect student focus based on face presence. The system uses OpenCV’s Haar Cascade Classifier to detect faces in real-time from a webcam feed and Pyttsx3 for audio alerts if the student appears unfocused.

## Features

- Real-time face detection using OpenCV and Haar Cascade Classifier.
- Voice feedback using Pyttsx3, alerting when no face is detected (indicating the student might not be focused).
- Customizable parameters for detection accuracy and alert frequency.

## Prerequisites

- Python 3.x
- OpenCV
- Pyttsx3
- Numpy

Install the dependencies using:

```bash
pip install opencv-python-headless pyttsx3 numpy
```
## How to Run
  1. Make sure a webcam is connected.
  2. Run the script: `python focus_detection.py`
  3. A window named “Student” will open, showing a rectangle around detected faces. If no face is detected, a voice prompt will alert that the student is not focused.
  4. Press “q” to quit the application.

## Future Improvements
- **Enhanced Focus Detection**: Add eye-tracking functionality to better assess focus by detecting if eyes are closed or averted.
- **Data Logging**: Implement a logging mechanism to track focus patterns over time, potentially storing timestamps and duration of inattentiveness for further analysis.
- **Multi-Student Support**: Expand the system to handle multiple faces, useful for group settings or classrooms.
- **Improved Voice Feedback**: Allow customizable messages or audio tones based on the detected face’s behavior, with configurable intervals for repetitive alerts.
- **Emotion Recognition**: Use a more advanced model to assess facial expressions, identifying emotions like boredom or distraction.
- **GUI Integration**: Add a simple graphical interface to make it user-friendly, allowing users to configure settings directly.
