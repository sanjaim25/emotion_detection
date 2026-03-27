# 😊 Emotion Detection System

A Flask-based web application that detects human emotions from images using DeepFace. Upload an image or capture one directly from your webcam to identify emotions in real-time.

## ✨ Features

- 📤 Upload images for emotion analysis
- 📸 Real-time webcam capture
- 🎭 Detects 7 emotions: Happy, Sad, Angry, Surprise, Fear, Disgust, Neutral
- 😭 Smart detection for complex emotions (e.g., crying)
- 🚫 Validates human face presence
- 😀 Visual emoji feedback for detected emotions

## 🛠️ Tech Stack

- **Backend**: Flask (Python)
- **ML Framework**: DeepFace
- **Computer Vision**: OpenCV
- **Frontend**: HTML, CSS, JavaScript


## 📁 Project Structure

```
.
├── app.py                  # Main Flask application
├── requirements.txt        # Python dependencies
├── model/
│   └── emotion_model.h5   # Pre-trained model (if applicable)
├── static/
│   ├── style.css          # Styling
│   ├── upload.jpg         # Uploaded image storage
│   └── capture.jpg        # Captured image storage
└── templates/
    ├── index.html         # Home page
    └── result.html        # Results display page
```

## 🎯 How It Works

1. **Upload Mode**: Select an image file from your device
2. **Capture Mode**: Use your webcam to take a photo
3. The system analyzes the image using DeepFace
4. Displays the detected emotion with a corresponding emoji
5. Shows confidence scores for all emotions

## 🧠 Emotion Detection Logic

- Uses DeepFace's pre-trained models for facial emotion recognition
- Enforces strict face detection to avoid false positives
- Implements custom logic for complex emotions (e.g., crying detection)
- Returns "Not a Human Face ❌" if no valid face is detected

## 📦 Dependencies

```
flask
tensorflow
opencv-python
numpy
deepface


