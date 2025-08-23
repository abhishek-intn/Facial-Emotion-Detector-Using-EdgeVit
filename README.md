# Facial-Emotion-Detector-Using-EdgeVit
Facial Emotion Detection system using EdgeViT, trained to classify 7 emotions (Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral). Optimized for real-time performance on edge devices like Raspberry Pi with live inference via OpenCV. Lightweight yet accurate deep learning model.
Real-Time Emotion Recognition using EdgeViT-XXS

This project implements a real-time emotion recognition system using a webcam, EdgeViT-XXS Transformer model, and MediaPipe face detection.
It captures live video, detects faces, applies frequency-based preprocessing, and classifies facial emotions into seven categories:

😡 Angry

🤢 Disgust

😨 Fear

😀 Happy

😐 Neutral

😢 Sad

😲 Surprise

🚀 Features

Real-time face detection using MediaPipe

Emotion classification with EdgeViT-XXS (Vision Transformer)

Frequency-domain preprocessing (Low-pass + High-pass filters)

Dynamic quantization for optimized inference on CPU / Raspberry Pi

Live FPS counter and probability bar visualization

📂 Project Structure
.
├── emotion_app.py         # Main script (your uploaded code)
├── edgevit-xxs_finetuned.pth  # Pretrained model (not included, add your own)
└── README.md              # Documentation

⚙️ Requirements

Install dependencies using pip:

pip install torch torchvision mediapipe opencv-python pillow numpy

▶️ Usage

Clone this repository:

git clone https://github.com/yourusername/emotion-recognition.git
cd emotion-recognition


Place your finetuned EdgeViT-XXS model (edgevit-xxs_finetuned.pth) inside the project folder.

Run the application:

python emotion_app.py


Press q to quit the webcam window.

🎥 Output

Live webcam feed with detected face bounding boxes

Emotion prediction displayed above the face

Probability bars for all emotion categories

FPS counter for performance monitoring

Extra debug window showing frequency transformed face image

🖥️ Example Screenshot

<img width="562" height="417" alt="Screenshot 2025-05-05 011018" src="https://github.com/user-attachments/assets/fecdc290-7982-418a-98ca-9dc89182844e" />


🔮 Future Improvements

Deploy as a lightweight Raspberry Pi application

Support for multi-face detection

Integration with Flask/Streamlit for web-based emotion recognitio
