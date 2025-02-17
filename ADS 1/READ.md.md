# Handling Class Imbalance in Breast Cancer Classification
This project explores techniques for addressing class imbalance in machine learning using the Breast Cancer dataset from the sklearn library. It focuses on enhancing the detection of malignant tumors (minority class) through resampling techniques like SMOTE and cost-sensitive learning using RandomForestClassifier.

---

## Table of Contents
1. [Abstract](#abstract)
2. [Problem Statement](#problem-statement)
3. [Techniques Used](#techniques-used)
4. [Data Preprocessing](#data-preprocessing)
5. [Model Implementation](#model-implementation)
6. [Evaluation Metrics](#evaluation-metrics)
7. [Conclusion](#conclusion)
8. [Installation and Setup](#installation-and-setup)
9. [References](#references)

---

## Abstract
This notebook investigates the challenge of class imbalance in breast cancer classification. Using SMOTE for oversampling and adjusting class weights in the RandomForestClassifier, the model aims to improve recall for malignant tumors while maintaining overall performance. Key metrics used for evaluation include F1-score, AUROC, and confusion matrices.

---

## Problem Statement
The primary objective is to enhance the performance of a classifier in detecting malignant tumors, the minority class in the Breast Cancer dataset. Without proper handling of class imbalance, models often exhibit low recall for this class, leading to false negatives.

---

## Techniques Used
- **Synthetic Minority Oversampling Technique (SMOTE)**: Generates synthetic samples to balance the class distribution.
- **Cost-Sensitive Learning**: Adjusts class weights to give more importance to the minority class.
- **RandomForestClassifier**: Used for baseline and improved models.
- **StandardScaler**: For feature normalization.

---

## Data Preprocessing
1. **Data Loading**: Using the inbuilt Breast Cancer dataset from sklearn.
2. **Data Normalization**: Features are standardized using StandardScaler.
3. **Handling Class Imbalance**: Applied SMOTE to generate synthetic samples for the minority class.
4. **Train-Test Split**: Split the dataset into training and testing sets using a 70:30 ratio.

---

## Model Implementation
1. **Baseline Model**: RandomForestClassifier without handling class imbalance.
2. **Improved Model**: Applied SMOTE and adjusted class weights in the RandomForestClassifier.

---

## Evaluation Metrics
- **F1-Score**: To balance precision and recall.
- **AUROC (Area Under Receiver Operating Characteristic)**: To measure the model's performance in distinguishing classes.
- **Confusion Matrix**: To visualize True Positives, False Positives, True Negatives, and False Negatives.

---

## Conclusion
This project demonstrates the effectiveness of resampling techniques and cost-sensitive learning in addressing class imbalance. By applying SMOTE and adjusting class weights, the model achieves better recall for malignant tumors without compromising overall accuracy.

---

## Installation and Setup
1. Clone this repository:
    ```bash
    git clone <repository-url>
    ```
2. Install required packages:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebook:
    ```bash
    jupyter notebook Assignment_1_002840576.ipynb
    ```

---

## References
- Chawla et al. (2002). **SMOTE: Synthetic Minority Over-sampling Technique.**
- Batista et al. (2004). **A Study of the Behavior of Several Methods for Balancing Machine Learning Training Data.**
- Galar et al. (2011). **Ensemble learning for imbalanced data sets: A review.**
