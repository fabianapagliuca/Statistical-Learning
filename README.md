Breast Cancer Classification Project
Author: Fabiana Pagliuca
Date: April 1, 2024
Course: Statistical Learning
🧠 Overview
This project focuses on the classification of breast tumors as either malignant (cancerous) or benign (non-cancerous) using machine learning techniques. The dataset consists of 30 numerical features derived from cell nuclei measurements via digitized images.
📊 Dataset
Source: breast-cancer1.xlsx
Instances: 539 observations
Attributes:
ID
Diagnosis: M (malignant) / B (benign)
30 numerical features, each describing:
Mean
Standard Error (SE)
Worst (mean of the three largest values)
Features represent characteristics such as:
Radius
Texture
Perimeter
Area
Smoothness
Compactness
Concavity
Symmetry
Fractal dimension
🧼 Data Cleaning & Preprocessing
Removed highly correlated variables (threshold > 0.9)
Handled class imbalance through undersampling
Rescaled features
Converted diagnosis column into a factor:
0 = Malignant
1 = Benign
🔎 Exploratory Data Analysis
Examined class distribution
Correlation matrix analysis
Identified key variables
Applied Principal Component Analysis (PCA)
Retained 8 principal components (explained variance > 85%)
🤖 Machine Learning Models
The following models were trained and evaluated on both the original dataset and the PCA-reduced dataset:
Logistic Regression
Random Forest
K-Nearest Neighbors (KNN)
Support Vector Machine (SVM)
Decision Tree
Gradient Boosting (GBM)
📈 Evaluation Metrics
Accuracy
Precision
Sensitivity
Confusion Matrix
ROC Curve & AUC
🏆 Results
Model	Original Dataset	PCA Dataset
Random Forest	91.5% accuracy	90.4% accuracy
KNN	90.4% accuracy	87.2% accuracy
SVM	80.0% accuracy	84.0% accuracy
Decision Tree	87.2% accuracy	84.0% accuracy
Random Forest was the most accurate across both datasets.
PCA reduced computational complexity while preserving high performance.
Key variables identified: Area Worst, Concave Points Worst, Concavity Mean, Area Mean, Radius Worst.
📌 Conclusion
Both datasets yielded strong predictive models, with the original features slightly outperforming PCA. However, PCA models demonstrated:
Reduced dimensionality
Faster computation
Comparable accuracy
Best Model: Random Forest (with or without PCA)
Recommendation: Use PCA for real-world implementations where computational efficiency is crucial.
