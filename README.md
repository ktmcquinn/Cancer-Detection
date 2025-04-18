# Cancer-Detection

# Metastatic Cancer Detection from Histopathologic Images

This project uses deep learning techniques to detect the presence of metastatic cancer in small histopathologic image patches. Built with TensorFlow/Keras and powered by transfer learning (ResNet50), the pipeline efficiently handles a large volume of high-resolution medical imagery for binary image classification.

## Project Overview

- **Dataset**: [Histopathologic Cancer Detection](https://www.kaggle.com/competitions/histopathologic-cancer-detection)
- **Task**: Binary classification of image patches as either **cancerous (1)** or **non-cancerous (0)**
- **Model**: Pretrained **ResNet50** with custom classification head
- **Tools**: Python, TensorFlow, Keras, Google Colab
- **Goal**: Predict cancer presence in test images and submit to Kaggle in the required format

---

## How to Run

You can run this notebook locally or on [Google Colab](https://colab.research.google.com/).

### Option 1: Run in Google Colab
Click the badge below to open in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your_username/your_repo/blob/main/notebook.ipynb)

1. Upload `histopathologic-cancer-detection.zip` (from Kaggle)
2. Follow the notebook steps to:
   - Unzip and load the dataset
   - Train the model
   - Predict on test images
   - Generate `submission.csv` file

### Option 2: Run Locally
1. Clone this repo  
2. Install dependencies  
   ```bash
   pip install -r requirements.txt
