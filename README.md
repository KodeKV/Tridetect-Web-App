# Tridetect: Multimodal Deepfake Detection System

## 📖 Table of Contents
- [Overview](#overview)
- [Key Features](#key-features)
- [Technologies Used](#technologies-used)
- [Datasets Used](#datasets-used)
- [Project Structure](#project-structure)
- [Setup](#setup)
- [Usage](#usage)
- [Video Demonstration](#video-demonstration)
- [License](#license)

## Overview
Tridetect is a powerful multimodal deepfake detection system designed to combat the growing threat of manipulated media. This project integrates cutting-edge deep learning techniques for identifying deepfakes in audio, images, and videos, ensuring digital content authenticity.

Deepfakes leverage AI to create hyper-realistic fake media that threaten individual privacy, organizational security, and societal trust. Tridetect provides a comprehensive solution to detect such manipulations using specialized models for each modality.

## Key Features
- **Audio Detection**: Utilizes an LSTM-based model to detect deepfake audio.
- **Image Detection**: Employs a fine-tuned VGG16 model to differentiate between real and fake images.
- **Video Detection**: Combines CNN and RNN approaches to identify manipulated video content.

## Technologies Used
- **Audio Deepfake Detection**:
Model: LSTM with MFCC features.
Capable of detecting temporal inconsistencies in synthesized audio.
- **Image Deepfake Detection**:
Model: Fine-tuned VGG16 with transfer learning.
Identifies visual inconsistencies in lighting, texture, and facial features.
- **Video Deepfake Detection**:
Model: Combined CNN and RNN.
Detects spatial and temporal inconsistencies across video frames.
- **Web App**:
Intuitive user interface to upload and classify media in real-time.
Supports audio (.wav), image (.jpg, .png), and video (.mp4, .avi) formats.

## Datasets Used
- **FaceForensics++**: A dataset consisting of manipulated videos created using different methods, used for video deepfake detection.
- **Celeb-DF (V1 & V2)**: A large-scale dataset of celebrity deepfake videos, used to improve model robustness.
- **Rohith ND's Fake and Real Audio Dataset**: A Kaggle dataset consisting of real and synthesized audio samples, used for audio deepfake detection.
- **Deepfake and Real Images by Manjil Karki**: A Kaggle dataset containing real and deepfake images, used for image detection models.

## Project Structure
/project-directory
├── /templates
│   ├── index.html
│   └── result.html
├── /static
│   ├── index.css
│   ├── result.css
│   └── /uploads
├── app.py
├── deepfake_audio_detection_model.h5
├── best_deepfake_model_final.keras
└── deepfake_video_11_12_model.h5

## Setup
- Prerequisites
Python 3.8 or higher
pip (Python package manager)

- Installation
1. Clone the Repository:
git clone https://github.com/KodeKV/Tridetect-Web-App.git
cd Tridetect-Web-App
2. Install Dependencies:
pip install -r requirements.txt
3. Run the Application:
python app.py
4. Access the Web Application: Open a web browser and navigate to http://localhost:5000.

## Usage
1. Upload media files (audio, image, or video) via the web interface.
2. The system processes the media and classifies it as "Real" or "Fake."
3. View classification results and confidence levels alongside media previews.

## Video Demonstration
Watch the web application in action:

![Tridetect GIF](https://github.com/KodeKV/Tridetect-Web-App/blob/main/Tridetect_recording_480p-MadewithClipchamp1-ezgif.com-video-to-gif-converter.gif)

## License
This project is licensed under the MIT License. You are free to use, modify, and distribute this software, provided that the original copyright notice and this permission notice are included in all copies or substantial portions of the software.

For detailed terms, see the LICENSE file in the repository.

