# Diabetes ML Classifier

A group project for CS364 — Machine Learning at IMSIU. Three machine learning classifiers are trained and compared to predict whether a patient is Diabetic, Non-Diabetic, or Pre-Diabetic based on clinical data.

---

## What This Project Does

Given a patient's clinical measurements, the model predicts one of three diabetes outcomes:
- Y — Diabetic
- N — Non-Diabetic
- P — Pre-Diabetic

Three classifiers were implemented and evaluated side by side: Decision Tree, SVM, and KNN.

---

## Dataset

1,000 patient records with 14 clinical features sourced from Mendeley Data.

Features include: Age, Gender, Urea, Cr, HbA1c, Cholesterol, TG, HDL, LDL, VLDL, BMI.

The dataset is included in the `Diabetes Dataset/` folder.

---

## Preprocessing

- Removed trailing whitespace from CLASS labels
- Standardised Gender column to uppercase
- Removed ID and No_Patient columns as they carry no predictive value
- Encoded Gender as 0 (M) and 1 (F)

---

## Models and Results

| Model | Accuracy | Precision | Recall |
|---|---|---|---|
| Decision Tree | 0.98 | 0.9805 | 0.98 |
| KNN | 0.90 | 0.888 | 0.90 |
| SVM | 0.845 | 0.714 | 0.845 |

Decision Tree was the best performing model. Feature importance analysis showed BMI (51.9%) and HbA1c (34.1%) together account for 86% of the model's decisions.

---


## Dependencies
scikit-learn
pandas
numpy
matplotlib
seaborn

---

## Authors
 Danah AlQarni, Munera AlZamil, Rawan AlOtaibi, Rzan AlSaadoun.

CS364 — Machine Learning | Dr. Dalal Aduwaila | IMSIU
