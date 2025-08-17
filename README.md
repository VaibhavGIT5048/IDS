# Anomaly Detection Benchmarking Project

## Overview

In this project, I conducted a comprehensive benchmarking and evaluation of multiple machine learning models to detect anomalies (attacks) in network traffic data. The objective was to identify which models perform best at distinguishing benign traffic from attacks, balancing high detection accuracy with low false alarm rates.

---

## What I Did

### 1. Data Preparation
- Loaded and cleaned network traffic datasets from multiple days.
- Selected key features representing network flow characteristics.
- Created a training dataset consisting only of benign (normal) samples.
- Prepared a test dataset containing both benign and attack samples.
- Applied preprocessing, feature transformations, and scaling.

### 2. Model Training and Evaluation
- Trained supervised models:  
  - XGBoost, LightGBM, CatBoost  
  - Random Forest  
  - k-Nearest Neighbors (k-NN)  

- Applied unsupervised/anomaly detection methods:  
  - Gaussian Mixture Model (GMM)  
  - Local Outlier Factor (LOF)  
  - One-Class Support Vector Machine (One-Class SVM)  
  - Autoencoder  

- Optimized classification thresholds for each model to maximize F1 score.

### 3. Metrics and Visualization
- Evaluated each model using F1 score, precision, recall, ROC AUC, and Average Precision (AP).
- Visualized confusion matrices showing model performance at best thresholds.
- Plotted ROC and Precision-Recall curves to assess ranking and discrimination ability.
- Produced comprehensive side-by-side comparisons for easy evaluation.

---

## What I Achieved

- Established a fair and consistent experimental framework for benchmarking diverse models.
- Identified CatBoost, Random Forest, and k-NN as best-performing models balancing detection and false alarms.
- Noted that XGBoost and LightGBM had high false positive rates at selected thresholds.
- Found unsupervised methods useful for anomaly ranking but less precise in classification compared to supervised models.
- Generated detailed visual insights to guide model selection and tuning.

---

## Why I Did This

- To tackle the challenge of detecting sophisticated cyber attacks in large network traffic data.
- To understand the trade-offs between maximizing attack detection and minimizing false positives.
- To select and tune effective anomaly detection models suitable for real-world deployment.
- To lay the groundwork for future improvements and operational deployment.

---

## Next Steps

- Perform hyperparameter tuning and model calibration on top-performing models.
- Explore ensemble techniques that combine strengths of multiple models.
- Test models on additional datasets and in real-time settings.
- Analyze feature importance to understand key drivers of detection.
- Collaborate with cybersecurity practitioners for deployment and feedback.

---

This project provides a solid foundation for building and deploying machine learning-based network anomaly detection systems with strong empirical validation and operational relevance.
