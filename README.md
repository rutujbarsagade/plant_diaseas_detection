# Plant Disease Detection using MobileNetV2

A deep learning model to classify plant leaf diseases using transfer learning with MobileNetV2.

## Features
- **38 disease classes** classification
- **MobileNetV2** pre-trained on ImageNet
- **87.97% validation accuracy** achieved
- Real-time inference capability
- Data augmentation for robust training

## Dataset
- **70,295 training images**
- **17,572 validation images**
- From Kaggle: [New Plant Diseases Dataset](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset)

## Model Architecture
- Input: 96×96 RGB images
- Base: MobileNetV2 (pre-trained)
- Custom layers:
  - Global Average Pooling
  - Dense(256) + BatchNorm + Dropout(0.4)
  - Dense(128) + Dropout(0.3)
  - Dense(38) softmax output
- Total params: 2,624,742

## Results
- Best validation accuracy: **87.97%**
- Final training accuracy: **87.32%**
- Training epochs: 10 (with early stopping)

## Installation
```bash
pip install tensorflow kagglehub matplotlib numpy
```
## Project Structure

├── plant_disease_detection.ipynb
├── best_model.keras
├── training_history.png
├── README.md
├── requirements.txt
└── .gitignore

🚀 Steps to Upload:
Create repo on GitHub

Clone locally:

bash
git clone https://github.com/rutujbarsagade/plant-disease-detection.git
cd plant-disease-detection
Add files:

bash
git add .
git commit -m "Initial commit: Plant disease detection model with 87.97% accuracy"
git push origin main
⚠️ IMPORTANT - Secure Your Credentials:

Remove Kaggle credentials from notebook before pushing
Add credentials handling via environment variables
Create a setup guide for users
🔐 Security Note:
Replace this in your notebook:

Python
KAGGLE_USERNAME = "your_username"
KAGGLE_KEY = "your_key"
With environment variables:

Python
import os
KAGGLE_USERNAME = os.getenv('KAGGLE_USERNAME')
KAGGLE_KEY = os.getenv('KAGGLE_KEY')
