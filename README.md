# Machine Learning for Cancer Diagnosis Prediction

This repository contains a machine learning project aimed at predicting whether a tumor is benign or malignant based on patient data. The primary algorithm used is **Logistic Regression**, which is well-suited for binary classification problems like cancer diagnosis.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Preprocessing](#preprocessing)
4. [Model Building](#model-building)
5. [Model Evaluation](#model-evaluation)
6. [Results](#results)
7. [Conclusion](#conclusion)
8. [Requirements](#requirements)
9. [How to Run](#how-to-run)
10. [References](#references)

---

## Project Overview

Cancer diagnosis is a critical task in the healthcare domain. This project utilizes a machine learning model to assist in classifying whether tumors are malignant or benign based on clinical data. We apply Logistic Regression to achieve this, leveraging key features from the dataset to train the model.

---

## Dataset

The dataset used in this project is based on breast cancer diagnostic data. Each row represents a patient's medical record, and the columns contain various features such as the mean radius, mean texture, area, smoothness, etc. The target variable is the **diagnosis**, which is labeled as either:
- **M (Malignant)**: Represented as 1.
- **B (Benign)**: Represented as 0.

---

## Preprocessing
Several preprocessing steps were applied to prepare the data for modeling:
1. **Dropping Irrelevant Columns**: 
   - The `id` and unnamed columns were removed, as they are not useful for prediction.

2. **Label Encoding**: 
   - The `diagnosis` column was converted into binary values (0 for benign, 1 for malignant).

3. **Scaling**: 
   - Feature scaling was applied using the `StandardScaler` to normalize the data and improve model performance.

4. **Train-Test Split**: 
   - The dataset was split into training (70%) and testing (30%) sets to evaluate the model’s performance on unseen data.

---

## Model Building
The following steps were performed to build the predictive model:

1. **Logistic Regression**:
   - A Logistic Regression model was chosen due to the binary nature of the target variable (benign vs malignant).
   - The model was trained on the scaled features of the training data.

---

## Model Evaluation
We evaluated the model using several metrics, including accuracy, precision, recall, and F1-score. These metrics help us understand the model's performance in distinguishing between benign and malignant cases.

- **Accuracy**: The overall proportion of correctly classified tumors.
  
- **Precision**: The proportion of true positives among all positive predictions.
  
- **Recall (Sensitivity)**: The ability of the model to detect malignant tumors correctly.

- **F1-Score**: The harmonic mean of precision and recall, giving a balanced measure of both.

---

## Results

- **Accuracy of the Model**: 98%
The model demonstrated high accuracy in predicting cancer diagnoses, with strong precision, recall, and F1-scores across both classes (benign and malignant).

---

## Conclusion
This project highlights the potential of **Logistic Regression** in the medical field, specifically for predicting cancer diagnoses. By using data preprocessing techniques such as feature scaling and label encoding, combined with effective model evaluation, we were able to achieve a high accuracy rate.

