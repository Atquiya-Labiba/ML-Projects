## Overview
This repository contains different Machine Learning Projects.

## Project 1
### Asteroid Threat Detection
This project focuses on predicting whether an asteroid is potentially hazardous to Earth using machine learning classification models. The dataset contains asteroid characteristics such as diameter, velocity, miss distance, and brightness (absolute magnitude).

### Dataset
- Dataset can be found from kaggle [here](https://www.kaggle.com/datasets/sameepvani/nasa-nearest-earth-objects)
- Dataset Size: 90,836 rows × 10 columns

### Workflow
**1. Data Preprocessing**
- Dropped irrelevant columns (id, name, orbiting_body, sentry_object)
- Encoded categorical labels
- Normalized features (Box-Cox transformation)
- Removed outliers via Z-score
- Imputed missing values with KNN Imputer

**2. Handling Imbalance**
- Class imbalance addressed with SMOTE oversampling
  
**3. Feature Scaling**
- Standardized numerical features using StandardScaler
  
**4. Models Implemented**
- AdaBoost
- Random Forest
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes
  
**5. Evaluation Metrics**
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
  
**6. Results**
![Confusion Matrix](Asteroid_Thread_Detection/results.png)

Random Forest (After SMOTE) is the best model with balanced accuracy and precision/recall.



