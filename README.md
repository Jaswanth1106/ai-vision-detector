# 🤖 AI Vision Object Detector

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15-orange.svg)](https://www.tensorflow.org/)
[![Flask](https://img.shields.io/badge/Flask-3.0-black.svg)](https://flask.palletsprojects.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> Real-time object detection web application powered by TensorFlow MobileNetV2 and WebRTC. Built for **Computer Vision Hackathon 2026**.

![AI Vision Detector](https://img.shields.io/badge/Status-Active-success)

---

## ✨ Features

- 🎥 **Real-time Camera Feed** - WebRTC-powered live video streaming
- 🤖 **AI Object Detection** - MobileNetV2 trained on ImageNet (1000+ classes)
- 🎯 **Top-5 Predictions** - Confidence scores for multiple objects
- ⚡ **Lightning Fast** - Optimized for real-time performance
- 🎨 **Modern UI** - Animated gradients, glassmorphism, smooth transitions
- 📊 **Analytics Dashboard** - Track scans and average confidence
- 📱 **Responsive Design** - Works on desktop and mobile browsers

---

## 🖼️ Screenshots

### Main Interface
Beautiful gradient UI with live camera feed and real-time detection results.

### Detection in Action
Shows top 5 predictions with confidence scores and animated scan effect.

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| **Backend** | Python 3.9+, Flask, Flask-CORS |
| **AI Model** | TensorFlow 2.15, Keras, MobileNetV2 |
| **Image Processing** | OpenCV, Pillow, NumPy |
| **Frontend** | HTML5, CSS3, Vanilla JavaScript |
| **Camera** | WebRTC API, MediaDevices |
| **Fonts** | Google Fonts (Inter) |

---

## 📦 Installation

### Prerequisites
- Python 3.9 or higher
- pip package manager
- Webcam/camera device
- Modern web browser (Chrome, Firefox, Safari, Edge)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Jaswanth1106/ai-vision-detector.git
   cd ai-vision-detector
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   python app.py
   ```

4. **Open in browser**
   Navigate to: **http://localhost:5000**

---

## 🚀 Usage

1. Click **"Start Camera"** to enable webcam access
2. Grant camera permissions in your browser
3. Show an object to the camera (try: phone, cup, laptop, etc.)
4. Click **"Detect Object"** to analyze
5. View AI predictions with confidence scores
6. Click **"Stop"** when finished

---

## 🧠 AI Model Details

### MobileNetV2 Architecture
- **Type:** Convolutional Neural Network (CNN)
- **Dataset:** ImageNet (1.4M images, 1000 object classes)
- **Input:** 224×224 RGB images
- **Output:** Top-5 class predictions with confidence scores
- **Accuracy:** ~71% top-1, ~90% top-5 on ImageNet
- **Speed:** Optimized for mobile and edge devices

### Detectable Objects (Examples)
- 🐕 Animals: dog, cat, bird, elephant, bear
- 🚗 Vehicles: car, bicycle, motorcycle, airplane, boat
- 💻 Electronics: laptop, phone, keyboard, mouse, remote
- ☕ Items: cup, bottle, glasses, watch, wallet
- 🍕 Food: pizza, banana, apple, orange, sandwich
- ...and 995+ more classes!

---

## 📁 Project Structure

```
ai-vision-detector/
├── backend/
│   ├── app.py              # Flask server & API routes
│   └── requirements.txt    # Python dependencies
├── frontend/
│   ├── index.html         # Main UI structure
│   ├── style.css          # Enhanced styling & animations
│   └── script.js          # Camera & detection logic
├── README.md              # This file
└── .gitignore            # Git ignore rules
```

---

## 🔌 API Documentation

### Health Check
```http
GET /api/health
```
**Response:**
```json
{
  "status": "healthy",
  "model": "MobileNetV2",
  "framework": "TensorFlow + Keras"
}
```

### Object Detection
```http
POST /api/detect
Content-Type: application/json

{
  "image": "data:image/jpeg;base64,..."
}
```

**Response:**
```json
{
  "success": true,
  "primary_object": "laptop",
  "confidence": 94.2,
  "detections": [
    {
      "label": "laptop",
      "confidence": 94.23,
      "class_id": "n03642806"
    },
    {
      "label": "notebook",
      "confidence": 3.12,
      "class_id": "n03832673"
    }
  ]
}
```

---

## 🎨 UI Features

- ✨ Animated gradient background with floating shapes
- 🎭 Glassmorphism design elements
- 📏 Scan animation effect during detection
- 📊 Animated confidence meter
- 🔴 Live camera status indicator
- 🎯 Ranked top-5 predictions list
- 📈 Real-time statistics dashboard
- 🌈 Smooth hover effects and transitions
- 📱 Fully responsive grid layout

---

## 🐛 Troubleshooting

### Camera Not Working
- Ensure camera permissions are granted in browser
- Check if another app is using the camera
- Try a different browser (Chrome recommended)

### Backend Connection Failed
- Verify Flask server is running on port 5000
- Check firewall settings
- Ensure dependencies are installed correctly

### Low Detection Accuracy
- Ensure good lighting conditions
- Hold object clearly in frame
- Try different angles
- Use objects from ImageNet classes

---

## 🤝 Contributing

This is a hackathon project, but contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📈 Future Enhancements

- [ ] Add custom object detection (YOLO/SSD)
- [ ] Support multiple object detection with bounding boxes
- [ ] Save detection history to database
- [ ] Export results to CSV/JSON
- [ ] Add voice announcements
- [ ] Implement face detection/recognition
- [ ] Mobile app version (React Native)
- [ ] Docker containerization
- [ ] Real-time video stream detection

---

## 📄 License

MIT License - feel free to use this project for learning and hackathons!

---

## 👨💻 Author

**Jaswanth**
- GitHub: [@Jaswanth1106](https://github.com/Jaswanth1106)
- Built for Computer Vision Hackathon 2026

---

## 🙏 Acknowledgments

- TensorFlow team for MobileNetV2
- ImageNet dataset creators
- Flask framework developers
- Google Fonts (Inter typeface)

---

## 📞 Support

If you encounter issues:
1. Check the [Troubleshooting](#-troubleshooting) section
2. Open an issue on GitHub
3. Review closed issues for solutions

---

**⭐ Star this repo if you found it useful!**

Built with ❤️ using TensorFlow, Flask, and WebRTC
