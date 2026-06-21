# README.md

# Comparative Study of Machine Learning Algorithms Using Orange Data Mining

Author - Nagaraj B S

## Project Overview

This project presents a comparative analysis of various Machine Learning algorithms implemented using **Orange Data Mining**. The study covers supervised learning (classification and regression) and unsupervised learning (clustering) using multiple benchmark and real-world datasets.

The objective is to evaluate algorithm performance across different data types and problem domains using standard evaluation metrics.

---

# Datasets and Algorithms

| Dataset               | Algorithm(s)                      | Learning Type  |
| --------------------- | --------------------------------- | -------------- |
| Cluster Dataset       | K-Means                           | Clustering     |
| Credit Card Dataset   | K-Means, DBSCAN                   | Clustering     |
| Drug Dataset          | Decision Tree                     | Classification |
| Heart Disease Dataset | Logistic Regression, KNN          | Classification |
| Housing Dataset       | Linear Regression, KNN Regression | Regression     |
| Iris Dataset          | KNN                               | Classification |
| Random Data Dataset   | K-Means, DBSCAN                   | Clustering     |
| Sales Dataset         | Artificial Neural Network (ANN)   | Classification |
| Tennis Dataset        | Naïve Bayes                       | Classification |
| Titanic Dataset       | Artificial Neural Network (ANN)   | Classification |
| Zoo Dataset           | SVM, KNN                          | Classification |

---

# Dataset Descriptions

## 1. Cluster Dataset

A synthetic dataset containing numerical observations used to evaluate clustering performance.

### Algorithm Used

* K-Means

### Results

| Clusters | Silhouette Score |
| -------- | ---------------- |
| 2        | **0.647**        |
| 3        | 0.536            |
| 4        | 0.531            |
| 5        | 0.558            |
| 6        | 0.502            |
| 7        | 0.470            |
| 8        | 0.409            |

### Observation

The highest silhouette score (**0.647**) was achieved with **2 clusters**, indicating strong cluster separation and compactness.

---

## 2. Credit Card Dataset

Contains customer spending and transaction behavior data used for customer segmentation.

### Algorithms Used

* K-Means
* DBSCAN

### K-Means Results

| Clusters | Silhouette Score |
| -------- | ---------------- |
| 2        | 0.208            |
| 3        | **0.252**        |
| 4        | 0.198            |
| 5        | 0.192            |
| 6        | 0.202            |
| 7        | 0.206            |
| 8        | 0.218            |

### DBSCAN Parameters

* Core Point Neighbors = 4
* Epsilon (Neighborhood Distance) = 2.77

### Observation

The dataset exhibits weak cluster separation. K-Means achieved its best score at **3 clusters (0.252)**. DBSCAN was used to identify density-based customer groups and potential outliers.

---

## 3. Drug Dataset

### Algorithm Used

* Decision Tree

### Results

| Metric    | Value |
| --------- | ----- |
| AUC       | 0.620 |
| Accuracy  | 0.600 |
| F1 Score  | 0.606 |
| Precision | 0.616 |
| Recall    | 0.600 |
| MCC       | 0.172 |

### Observation

Decision Tree provided moderate classification performance for predicting suitable drugs based on patient characteristics.

---

## 4. Heart Disease Dataset

### Algorithms Compared

* Logistic Regression
* KNN

### Logistic Regression Results

| Metric    | Value  |
| --------- | ------ |
| AUC       | 0.582  |
| Accuracy  | 0.789  |
| F1 Score  | 0.774  |
| Precision | 0.760  |
| Recall    | 0.789  |
| MCC       | -0.117 |

### KNN Results

| Metric    | Value  |
| --------- | ------ |
| AUC       | 0.637  |
| Accuracy  | 0.867  |
| F1 Score  | 0.815  |
| Precision | 0.769  |
| Recall    | 0.867  |
| MCC       | -0.040 |

### Observation

KNN outperformed Logistic Regression across most evaluation metrics, achieving **86.7% accuracy**.

---

## 5. Housing Dataset

### Algorithms Compared

* Linear Regression
* KNN Regression

### KNN Regression Results

| Metric | Value   |
| ------ | ------- |
| MSE    | 4833.44 |
| RMSE   | 69.52   |
| MAE    | 45.80   |
| MAPE   | 13.84   |
| sMAPE  | 13.06   |
| R²     | 0.821   |

### Linear Regression Results

| Metric | Value   |
| ------ | ------- |
| MSE    | 2981.19 |
| RMSE   | 54.60   |
| MAE    | 36.50   |
| MAPE   | 11.29   |
| sMAPE  | 11.13   |
| R²     | 0.890   |

### Observation

Linear Regression significantly outperformed KNN Regression, producing lower prediction errors and a higher **R² score of 0.890**.

---

## 6. Iris Dataset

### Algorithm Used

* KNN

### Results

| Metric    | Value |
| --------- | ----- |
| AUC       | 0.982 |
| Accuracy  | 0.978 |
| F1 Score  | 0.978 |
| Precision | 0.979 |
| Recall    | 0.978 |
| MCC       | 0.966 |

### Observation

KNN achieved excellent performance on the Iris dataset with nearly perfect classification accuracy.

---

## 7. Random Data Dataset

### Algorithms Compared

* K-Means
* DBSCAN

### K-Means Results

| Clusters | Silhouette Score |
| -------- | ---------------- |
| 2        | 0.440            |
| 3        | 0.497            |
| 4        | 0.518            |
| 5        | **0.532**        |
| 6        | 0.527            |
| 7        | 0.518            |
| 8        | 0.499            |

### DBSCAN Parameters

| Parameter            | Value |
| -------------------- | ----- |
| Core Point Neighbors | 4     |
| Epsilon              | 0.19  |

### Observation

K-Means performed best with **5 clusters** (silhouette score = 0.532). DBSCAN identified density-based structures using ε = 0.19.

---

## 8. Sales Dataset

### Algorithm Used

* Artificial Neural Network (ANN)

### Results

| Metric    | Value |
| --------- | ----- |
| AUC       | 0.500 |
| Accuracy  | 0.547 |
| F1 Score  | 0.386 |
| Precision | 0.299 |
| Recall    | 0.547 |
| MCC       | 0.000 |

### Observation

The ANN model showed limited predictive capability, suggesting the need for additional preprocessing, feature engineering, or parameter tuning.

---

## 9. Tennis Dataset

### Algorithm Used

* Naïve Bayes

### Results

| Metric    | Value |
| --------- | ----- |
| AUC       | 0.759 |
| Accuracy  | 0.636 |
| F1 Score  | 0.635 |
| Precision | 0.641 |
| Recall    | 0.636 |
| MCC       | 0.329 |

### Observation

Naïve Bayes achieved moderate classification performance and effectively handled categorical tennis match attributes.

---

## 10. Titanic Dataset

### Algorithm Used

* Artificial Neural Network (ANN)

### Results

| Metric    | Value |
| --------- | ----- |
| AUC       | 0.766 |
| Accuracy  | 0.800 |
| F1 Score  | 0.765 |
| Precision | 0.830 |
| Recall    | 0.800 |
| MCC       | 0.493 |

### Observation

The ANN model performed well in predicting passenger survival with **80% accuracy**.

---

## 11. Zoo Dataset

### Algorithms Compared

* KNN
* SVM

### KNN Results

| Metric    | Value |
| --------- | ----- |
| AUC       | 0.999 |
| Accuracy  | 0.900 |
| F1 Score  | 0.872 |
| Precision | 0.860 |
| Recall    | 0.900 |
| MCC       | 0.874 |

### SVM Results

| Metric    | Value |
| --------- | ----- |
| AUC       | 0.997 |
| Accuracy  | 0.967 |
| F1 Score  | 0.962 |
| Precision | 0.971 |
| Recall    | 0.967 |
| MCC       | 0.958 |

### Observation

SVM achieved the best overall performance with **96.7% accuracy**, outperforming KNN on the Zoo dataset.

---

# Comparative Analysis

## Best Classification Model

| Dataset       | Best Algorithm | Accuracy |
| ------------- | -------------- | -------- |
| Drug          | Decision Tree  | 60.0%    |
| Heart Disease | KNN            | 86.7%    |
| Iris          | KNN            | 97.8%    |
| Tennis        | Naïve Bayes    | 63.6%    |
| Titanic       | ANN            | 80.0%    |
| Zoo           | SVM            | 96.7%    |

---

## Best Regression Model

| Dataset | Best Algorithm    | R²    |
| ------- | ----------------- | ----- |
| Housing | Linear Regression | 0.890 |

---

## Best Clustering Results

| Dataset         | Algorithm | Optimal Clusters | Silhouette Score |
| --------------- | --------- | ---------------- | ---------------- |
| Cluster Dataset | K-Means   | 2                | 0.647            |
| Credit Card     | K-Means   | 3                | 0.252            |
| Random Data     | K-Means   | 5                | 0.532            |

---

# Conclusion

This comparative study demonstrates that algorithm performance is highly dependent on dataset characteristics.

### Key Findings

* **KNN** achieved excellent performance on Iris and Heart Disease datasets.
* **SVM** delivered the highest classification accuracy on the Zoo dataset.
* **Linear Regression** outperformed KNN Regression for housing price prediction.
* **K-Means** successfully identified optimal cluster structures in synthetic and random datasets.
* **ANN** performed well on Titanic data but showed limited effectiveness on the Sales dataset.
* **Naïve Bayes** provided acceptable performance for categorical sports data.
* **Decision Trees** offered interpretable but moderate performance on drug prediction tasks.

Overall, the study highlights the importance of selecting algorithms based on dataset characteristics rather than relying on a single model for all tasks.

---

## Software Used

* Orange Data Mining
* Machine Learning Algorithms:

  * K-Means
  * DBSCAN
  * Decision Tree
  * Logistic Regression
  * KNN
  * Linear Regression
  * Naïve Bayes
  * Support Vector Machine (SVM)
  * Artificial Neural Network (ANN)

## Author - Nagaraj B S

Comparative Study of Machine Learning Algorithms Using Multiple Datasets – Orange Data Mining Project.
"# Data-Analytics-with-ML" 
