# Tridetect: Detecting Deepfakes in Audio, Video, and Images

Tridetect is a comprehensive solution designed to detect deepfake content in audio, images, and videos. The project leverages advanced machine learning models to ensure the authenticity of digital media, helping to mitigate the risks posed by synthetic media manipulation.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Datasets Used](#datasets-used)
- [Project Structure](#project-structure)
- [Setup](#setup)
- [Usage](#usage)
- [Video Demonstration](#video-demonstration)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Deepfakes have emerged as a significant threat in the digital age, with the potential to spread misinformation and undermine trust in digital content. Tridetect provides a reliable solution to identify and mitigate the impact of deepfakes, ensuring the integrity of audio, video, and image content.

## Features
- **Audio Detection**: Utilizes an LSTM-based model to detect deepfake audio.
- **Image Detection**: Employs a fine-tuned VGG16 model to differentiate between real and fake images.
- **Video Detection**: Combines CNN and RNN approaches to identify manipulated video content.

## Technologies Used
- **Python**
- **TensorFlow/Keras**
- **Flask** (for web interface)
- **Librosa**
- **OpenCV**

## Datasets Used
- **FaceForensics++**: A dataset consisting of manipulated videos created using different methods, used for video deepfake detection.
- **Celeb-DF (V1 & V2)**: A large-scale dataset of celebrity deepfake videos, used to improve model robustness.
- **Rohith ND's Fake and Real Audio Dataset**: A Kaggle dataset consisting of real and synthesized audio samples, used for audio deepfake detection.
- **Deepfake and Real Images by Manjil Karki**: A Kaggle dataset containing real and deepfake images, used for image detection models.

## Project Structure
/project-directory │ ├── /templates │ ├── index.html │ └── result.html ├── /statics │ ├── index.css │ ├── result.css │ └── /uploads ├── app.py ├── deepfake_audio_detection_model.h5 ├── best_deepfake_model_final.keras └── deepfake_video_11_12_model.h5
