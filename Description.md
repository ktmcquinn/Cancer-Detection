# Data Description

* **train_labels.csv**: Image IDs and binary cancer labels
* **train/**: ~220k .tif images for training
* **test/**: ~75k .tif images for prediction
* **sample_submission.csv**: file with required format for Kaggle submission

# Model Architecture 

Input (224x224x3)<br>
↓<br>
ResNet50 (pre-trained on ImageNet, frozen)<br>
↓<br>
GlobalAveragePooling2D<br>
↓<br>
Dense(256, ReLU)<br>
↓<br>
Dropout(0.5)<br>
↓<br>
Dense(1, Sigmoid) → Cancer Probability<br>

**Loss Function:** Binary Cross-Entropy<br>
**Optimizer:** Adam<br>
**Val Metrics:** Accuracy<br>

# Results
|Metric|Value|
|------|------|
|Train Accuracy|75.80%|
|Validation Accuracy|76.75%|
|Train Loss|51.09%|
|Validation Loss|50.25%|
|Kaggle Submission Score|**77.83%**|

# Acknowledgments
* Kaggle: Histopathologic Cancer Detection Dataset
* * Pre-trained ResNet50 provided by Keras Applications
