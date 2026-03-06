# Trustworthy Human Activity Recognition (HAR)

A reliability-aware machine learning pipeline that improves prediction trust using calibration, uncertainty estimation, and selective prediction.

## Problem

Traditional ML models always output predictions even when uncertain.

This project introduces a **trust-aware ML pipeline** that can:

• Accept confident predictions
• Defer difficult cases to a stronger model
• Reject uncertain predictions

## Dataset

UCI HAR Dataset

Activities:

* Walking
* Walking Upstairs
* Walking Downstairs
* Sitting
* Standing
* Laying

Features: **561**

Train Samples: **7352**
Test Samples: **2947**

## Models Used

* Logistic Regression
* Random Forest
* XGBoost

## Reliability Techniques

* Expected Calibration Error (ECE)
* Temperature Scaling
* Isotonic Regression
* Selective Prediction

## Custom Metric

TPS — Trustworthy Prediction Score

TPS = (Coverage × Selective Accuracy) / (1 + ECE)

## Results

Baseline Logistic Regression Accuracy

**95.9%**

Selective Prediction Engine

Coverage: **99.6%**
Selective Accuracy: **96.54%**
TPS: **0.9556**

## Tech Stack

Python
Scikit-Learn
XGBoost
SHAP
Matplotlib
Seaborn

## Future Improvements

* Real-time activity detection
* Streamlit dashboard
* API deployment
