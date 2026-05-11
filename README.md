# Power System Fault Detection and Classification Using Ensemble Machine Learning Methods

This repository contains the final code, datasets, report, and presentation for the MYZ307E Machine Learning for Electrical and Electronics Engineering term project.

## Project Description

The project focuses on machine learning-based fault detection and classification in three-phase power transmission systems using current and voltage measurements.

Two tasks are studied:

1. Binary fault detection: Normal vs. Fault
2. Six-class fault classification: No Fault, LG, LL, LLG, LLL, LLLG

## Datasets

### Dataset 1: Detection Dataset
- File: `powerline_dataset.csv`
- Samples: 12,001
- Features: Ia, Ib, Ic, Va, Vb, Vc
- Target: Output (S)
- Class distribution:
  - Normal: 6505 samples
  - Fault: 5496 samples

### Dataset 2: Classification Dataset
- File: `classData.csv`
- Samples: 7,861
- Features: Ia, Ib, Ic, Va, Vb, Vc
- Label columns: G, C, B, A
- Classes:
  - No Fault: 2365
  - LG: 1129
  - LL: 1004
  - LLG: 1134
  - LLL: 1096
  - LLLG: 1133

## Models Used

- SVM
- Decision Tree
- Random Forest
- KNN
- Naive Bayes
- Logistic Regression
- Gradient Boosting
- MLP
- Voting Ensemble
- GMM anomaly detection
- PCA analysis

## Final Results

### Fault Detection
Best model: Voting Ensemble  
Accuracy: 99.75%

### Fault Classification
Best model: Random Forest  
Accuracy: 88.24%

### GMM Anomaly Detection
Accuracy: 98.08%

### PCA
4 components preserve 96.9% variance.

## Files

- `Power_System_Fixed_v2.ipynb`: Main notebook
- `powerline_dataset.csv`: Detection dataset
- `classData.csv`: Classification dataset
- `FinalReport_FINAL.docx`: Final report
- `Presentation_FINAL.pptx`: Final presentation

## References

- T. Anwar, C. Mu, M. Z. Yousaf et al., "Robust fault detection and classification in power transmission lines via ensemble ML," Scientific Reports, 2025.
- https://github.com/svdeepak99/Machine_Learning-Power_System_Fault_Detection
- https://github.com/KingArthur000/Electrical-Fault-detection-and-classification