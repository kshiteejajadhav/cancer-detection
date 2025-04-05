# Cancer Detection using SVM

This project applies a Support Vector Machine (SVM) model to classify cell samples as **Benign (2)** or **Malignant (4)** using medical data from `cell_samples.csv`.

---

## Objective
To develop a binary classification model that can assist in the detection of cancerous cells using key biological features.

---

## Dataset
The dataset `cell_samples.csv` contains 9 attributes extracted from cell images:
- Clump Thickness
- Uniformity of Cell Size
- Uniformity of Cell Shape
- Marginal Adhesion
- Single Epithelial Cell Size
- Bare Nuclei
- Bland Chromatin
- Normal Nucleoli
- Mitoses

The `Class` column is the target:
- `2`: Benign
- `4`: Malignant

---

##  How It Works

1. Loads and cleans dataset
2. Extracts features and target variable
3. Trains an SVM (linear kernel)
4. Evaluates using accuracy, confusion matrix, precision, recall

---

## Results
- Classifier: SVM (Linear Kernel)
- Accuracy: ~`96%` 
- Evaluation:
                      `precision``recall`  `f1-score` `support`
      
                 2       1.00      0.94      0.97        90
                 4       0.90      1.00      0.95        47
      
          accuracy                           0.96       137
         macro avg       0.95      0.97      0.96       137
      weighted avg       0.97      0.96      0.96       137

---

## Setup

### Requirements
Install dependencies via:

```bash
pip install -r requirements.txt
