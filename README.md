# 🎗️ Breast Cancer Diagnosis Using Machine Learning

## Overview

This project explores the Breast Cancer Wisconsin Diagnostic Dataset to investigate whether machine learning models can distinguish between benign and malignant breast tumors using measurements extracted from digitized images of fine needle aspirates (FNA) of breast masses.

Rather than focusing only on model performance, this project emphasizes understanding the data, interpreting biomedical features, and comparing different machine learning algorithms.

---

## Research Question

**Can morphological characteristics of breast cell nuclei accurately distinguish between benign and malignant tumors using machine learning?**

---

## Dataset

* **Dataset:** Breast Cancer Wisconsin Diagnostic Dataset
* **Original Dataset:** UCI Machine Learning Repository – Breast Cancer Wisconsin Diagnostic Dataset
* **Accessed via:** https://www.kaggle.com/datasets/remyz5/curated-healthcare-and-genomics-datasets
* **Source:** *(Add the Kaggle dataset link here)*
* **Samples:** 569
* **Features:** 30 numerical predictor variables and 1 target variable
* **Target Variable:** `target`

  * 1 = Benign
  * 0 = Malignant

### Predictor Variables

The dataset contains measurements describing cell nuclei extracted from digitized images of breast masses, including:

* Radius
* Texture
* Perimeter
* Area
* Smoothness
* Compactness
* Concavity
* Concave Points
* Symmetry
* Fractal Dimension

During the data exploration phase, an inconsistency was identified in the dataset description regarding the target labels. The correct class encoding was verified using the original UCI Machine Learning Repository documentation before proceeding with the analysis.

---

## Objectives

* Explore the characteristics of breast tumor data.
* Understand the biological meaning of the extracted features.
* Perform Exploratory Data Analysis (EDA).
* Investigate relationships between variables.
* Train and compare multiple machine learning models.
* Interpret the results from both a machine learning and healthcare perspective.

---

## Project Workflow

### 1. Data Exploration

* Loaded and inspected the dataset.
* Examined data types and summary statistics.
* Verified the target distribution.
* Confirmed the correct target encoding using the original dataset documentation.

### 2. Data Cleaning

* Checked for missing values.
* Checked for duplicate observations.
* Verified that the dataset required no additional cleaning.

### 3. Exploratory Data Analysis (EDA)

Performed visual analysis using:

* Histograms
* Boxplots
* Correlation heatmaps

Key observations included:

* Malignant tumors generally have larger nuclei.
* Mean concavity strongly differentiates malignant and benign tumors.
* Several size-related features are highly correlated.
* The dataset exhibits clear biological patterns suggesting strong predictive potential.

### 4. Data Preprocessing

* Split the dataset into training and testing sets.
* Applied feature standardization where appropriate.

### 5. Machine Learning Models

The following classification models were trained and compared:

* Logistic Regression
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)

Each model was evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

---

## Model Comparison

| Model                            | Test Accuracy | Interpretation                                                       |
| -------------------------------- | ------------: | -------------------------------------------------------------------- |
| Logistic Regression              |       **97%** | Excellent performance with strong interpretability.                  |
| Decision Tree                    |       **94%** | Perfect training accuracy but showed clear overfitting.              |
| Random Forest                    |       **96%** | Reduced overfitting while maintaining strong predictive performance. |
| **Support Vector Machine (SVM)** |       **98%** | Best overall performance and excellent generalization.               |

---

## Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Training and testing accuracy were also compared to assess model generalization and detect overfitting.

---

## Key Concepts Learned

Through this project, I learned:

* The importance of Exploratory Data Analysis before model training.
* Why highly correlated features may contain redundant information.
* How feature scaling affects different machine learning algorithms.
* The difference between training accuracy and testing accuracy.
* How overfitting occurs in Decision Trees.
* Why ensemble methods such as Random Forest improve robustness.
* Why model evaluation should consider recall and confusion matrices rather than accuracy alone, especially in healthcare applications.
* How model coefficients and feature importance provide different perspectives for interpreting machine learning models.
* The importance of combining biomedical understanding with machine learning analysis.

---

## Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

---

## About This Project

This project demonstrated that machine learning models can effectively classify breast tumors using morphological characteristics of cell nuclei. More importantly, it reinforced the importance of combining data exploration, biological interpretation, and rigorous model evaluation to develop trustworthy healthcare AI solutions.

This project is part of my journey to build AI and data literacy in healthcare through hands-on analysis of biomedical datasets and machine learning.

---

## Acknowledgments

* Original dataset: UCI Machine Learning Repository – Breast Cancer Wisconsin Diagnostic Dataset.
* Curated dataset accessed through Kaggle.
