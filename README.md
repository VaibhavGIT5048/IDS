Anomaly Detection Benchmarking Project
Overview
In this project, I conducted a thorough benchmarking and evaluation of multiple machine learning models to detect anomalies (attacks) in network traffic data. My goal was to identify which models perform best at distinguishing benign traffic from attacks, balancing detection accuracy with false alarm rates.
What I Did
1. Data Preparation
Loaded and cleaned network traffic datasets from multiple days.
Selected relevant features representing flow characteristics.
Prepared a training set consisting only of benign examples (normal traffic).
Created a test set containing both benign and attack samples.
Applied necessary transformations and scaling to features for optimal model performance.
2. Model Training and Evaluation
Trained a variety of supervised classifiers:
XGBoost, LightGBM, CatBoost
Random Forest
k-Nearest Neighbors (k-NN)
Applied unsupervised/anomaly detection techniques:
Gaussian Mixture Model (GMM)
Local Outlier Factor (LOF)
One-Class Support Vector Machine (One-Class SVM)
Autoencoder
Tuned each model to find the best classification threshold that maximizes the F1 score, balancing precision and recall.
3. Metrics and Visualizations
Computed classification metrics including F1 scores, precision, recall, and accuracy.
Plotted confusion matrices at best thresholds for each model to visualize true positive/false positive trade-offs.
Created ROC and Precision-Recall (PR) curves to evaluate model discrimination and ranking capability.
Compared models visually in side-by-side grids for clear comparative analysis.
What I Achieved
Comprehensive Benchmarking: Evaluated 8+ models under the same experimental setup for a fair and consistent comparison.
Model Insight:
Identified CatBoost, Random Forest, and k-NN as top performers with the best balance between high attack detection and manageable false alarms.
Observed that XGBoost and LightGBM, while powerful, produced high false positives at optimal thresholds, indicating need for further tuning.
Recognized unsupervised models (GMM, LOF, One-Class SVM) as valuable for anomaly ranking, but with generally lower classification precision when labeled data is available.
Detailed Visual and Quantitative Comparisons: Produced easy-to-interpret confusion matrices and ROC/PR plots for all models facilitating informed model selection.
Robust Thresholding: Determined optimal decision thresholds per model to maximize real-world applicability.
Why I Did This
Address the challenge of detecting sophisticated cyber-attacks within large volumes of network traffic by evaluating diverse machine learning methods.
Understand trade-offs between detecting all attacks versus limiting false alarms which is critical for practical deployment.
Select the most effective anomaly detection technique for the given dataset and problem context based on both accuracy and operational feasibility.
Establish a rigorous experimental framework enabling future model improvements, deployment decisions, and benchmarking of new algorithms.
Next Steps
Perform deeper hyperparameter tuning for promising models like CatBoost and Random Forest.
Investigate ensemble or stacking approaches combining strengths of several models.
Evaluate model performance on additional datasets and real-time streaming data.
Explore feature importance analysis to understand driving factors behind detection.
Collaborate with cybersecurity teams to deploy and monitor best models in production.
This project provided me with a solid empirical foundation to select, tune, and deploy effective machine learning models for network anomaly detection, balancing high detection rates with operational constraints on false alarms.
