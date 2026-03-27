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

## 📋 Prerequisites

- Python 3.7+
- pip package manager

## 🚀 Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd <project-folder>
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
python app.py
```

4. Open your browser and navigate to:
```
http://127.0.0.1:5000
```

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
```

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## 📄 License

This project is open source and available under the MIT License.

## 🐛 Troubleshooting

- **Camera not working**: Ensure browser permissions are granted for camera access
- **Model errors**: DeepFace will automatically download required models on first run
- **Face not detected**: Ensure the image has a clear, front-facing human face

## 👨‍💻 Author

Created with ❤️ for emotion recognition
