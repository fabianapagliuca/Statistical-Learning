# Statistical-Learning

# Breast Cancer Classification Project

**Author:** Fabiana Pagliuca  
**Date:** 2024-04-01  

## Overview
This project aims to classify breast tumors as **malignant** (cancerous) or **benign** (non-cancerous) using machine learning models. The dataset includes 30 features extracted from cell nuclei images.

## Dataset
- **Attributes:** ID, Diagnosis (M/B), 30 numeric features (mean, SE, worst) of nucleus characteristics such as radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry.
- **Source:** `breast-cancer1.xlsx`

## Methods
1. **Data Cleaning & Preprocessing**  
   - Removed highly correlated variables  
   - Scaled data  
   - Converted diagnosis to factor (0 = malignant, 1 = benign)

2. **Exploratory Analysis**  
   - Correlation matrix  
   - Principal Component Analysis (PCA) for dimensionality reduction

3. **Machine Learning Models**  
   - Logistic Regression  
   - Random Forest  
   - K-Nearest Neighbors (KNN)  
   - Support Vector Machine (SVM)  
   - Gradient Boosting (GBM)  

4. **Evaluation Metrics**  
   - Confusion Matrix  
   - ROC Curve & AUC  

## Results
- PCA reduced dimensions while keeping >85% variance.  
- Random Forest and SVM achieved high accuracy.  
- Feature importance and model evaluation visualized with plots.

