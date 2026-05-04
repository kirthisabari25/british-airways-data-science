# British Airways Data Science — Task 2: Customer Booking Prediction

## Overview
Predictive model to identify customers likely to complete a flight booking,
built as part of the British Airways Forage Data Science Virtual Experience.

## Dataset
- 50,000 customer booking records
- 14 original features + 4 engineered features
- Target: `booking_complete` (14.96% positive class)

## Model
- Algorithm: Random Forest Classifier
- Trees: 100 | Max Depth: 10 | Class Weight: Balanced
- Validation: Stratified 3-Fold Cross-Validation

## Results
| Metric | Score |
|--------|-------|
| CV Accuracy | 69.7% |
| CV ROC-AUC | 0.677 |
| Test ROC-AUC | 0.681 |
| CV F1 Score | 33.9% |

## Top Predictors
1. Flight Duration — 23.7%
2. Length of Stay — 17.8%
3. Purchase Lead Time — 13.9%

## Files
- `notebook.ipynb` — Full analysis and model code
- `feature_importance.png` — Feature importance chart
- `roc_curve.png` — ROC curve (AUC = 0.681)
- `confusion_matrix.png` — Confusion matrix
- `BA_Task2_Booking_Prediction.pptx` — Summary slide

## Tools
Python · scikit-learn · pandas · matplotlib · Random Forest
