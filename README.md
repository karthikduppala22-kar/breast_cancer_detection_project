#Breast Cancer Detection Project

## Project Overview
This project predicts whether a breast cancer tumor is **Benign (B)** or **Malignant (M)** using machine learning models.  
It demonstrates the complete ML workflow, including data preprocessing, model training, evaluation, and visualization of performance metrics.

---

## Dataset
The dataset used is from **Kaggle**: [Breast Cancer Dataset](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset)

- **Number of samples:** 569  
- **Number of features:** 30 (numeric features)  
- **Target:** `B` (Benign) or `M` (Malignant)  

---

## Workflow

1. **Data Loading & Exploration**
   - Loaded CSV dataset
   - Checked for null values (none found)
   - Explored data distribution

2. **Data Preprocessing**
   - Converted target labels `B` → 0, `M` → 1 for binary classification
   - Split data into **train, validation, and test sets**
   - Scaled features for SVC and Logistic Regression

3. **Model Training**
   - Trained multiple classification models:
     - Logistic Regression
     - Decision Tree
     - Random Forest
     - Support Vector Classifier (SVC)
     
4. **Model Evaluation**
   - Evaluated models on **Test Set** using:
     - Accuracy
     - Precision, Recall, F1-score
     - Confusion Matrix
     - ROC–AUC Score
   - Plotted **separate ROC curves** for each model

---

## Results Summary

| Model                  | Accuracy | ROC–AUC | Notes |
|------------------------|----------|---------|-------|
| Logistic Regression    | 88.6%    | 0.950   | Good overall performance |
| Decision Tree          | 91.2%    | 0.902   | Slightly better than Logistic Regression |
| Random Forest          | 92.9%    | 0.978   | Best performance in all metrics |
| SVC                    | 59.6%    | 0.600   | Poor performance without proper scaling |

> Random Forest achieved the **highest accuracy and ROC–AUC** on the test set.  

---

## Visualization

- **ROC Curves:** Separate ROC–AUC curves were plotted for each model.  
- **Confusion Matrix:** Visualized in Jupyter Notebook for each model to understand misclassifications.

---

## Libraries Used
- pandas, numpy  
- scikit-learn  
- matplotlib 

---

## How to Run
1. Clone this repository:  
```bash
git clone https://github.com/karthikduppala-kar/breast_cancer_detection_project.git
