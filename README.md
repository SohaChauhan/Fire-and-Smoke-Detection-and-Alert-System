# Fire and Smoke Detection and Alert System

This project is a deep learning-based application for detecting fire and smoke in videos, with real-time alerting capabilities. It leverages object detection and tracking models to identify fire and smoke, and sends SMS alerts when an incident is detected.

## Features
- **Video Upload & Processing**: Upload MP4 videos for automatic fire and smoke detection.
- **Object Tracking**: Uses Deep SORT for real-time object tracking.
- **Alert System**: Sends SMS alerts using Twilio when fire or smoke is detected.
- **Streamlit Interface**: User-friendly web interface for uploading and processing videos.

## How It Works
1. **Upload** a video file via the Streamlit web interface.
2. The system processes the video using a YOLO model (`best.pt`) to detect fire and smoke.
3. Detected objects are tracked frame-by-frame.
4. If fire or smoke is detected, an SMS alert is sent using Twilio.
5. The processed video with detection overlays is displayed for download or review.


## File Structure
- `app.py` : Main Streamlit application
- `best.pt` : YOLO model weights
- `requirements.txt` : Python dependencies
- `packages.txt` : System dependencies (ffmpeg)
- `.env` : Environment variables for Twilio (not included)
