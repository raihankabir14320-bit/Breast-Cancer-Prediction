# Breast-Cancer-Prediction
This repository contains a machine learning project designed to classify breast cancer diagnoses as Malignant (M) or Benign (B) using the Breast Cancer Wisconsin dataset. The project demonstrates the application of both unsupervised and supervised learning techniques to solve a medical classification problem.
K-Nearest Neighbors (KNN) (Supervised Learning): This method builds a predictive model for classification.

Approach

1. Data Preprocessing

Encoding: The diagnosis column was changed from categorical to numerical values:

M (Malignant) becomes 1

B (Benign) becomes 0

Cleaning: Irrelevant columns (id and Unnamed: 32) were removed to reduce noise.

Normalization: Min-Max Normalization scaled all feature values between 0 and 1. This is important for KNN and K-Means since they are distance-based methods sensitive to data scale.

Splitting: The data was divided into 80% for training and 20% for testing.

2. K-Means Clustering

I used K-Means with k=2 to determine if the algorithm could separate Benign and Malignant cases without knowing the labels.

Observation: We compared the clustering results to the actual diagnosis labels using a cross-tabulation table.

3. K-Nearest Neighbors (KNN)

A KNN classifier was trained with k=5.

The model was tested on the unseen data set, which was 20% of the total data.

Results:

KNN Model Performance

Accuracy: 0.9649


Files

Dataset (1).csv: The raw dataset used for analysis.

Breast_Cancer_Prediction.ipynb: The Google Colab notebook containing the code.
Precision:  0.9535

Recall: 0.9649

F1-Score: 0.9535
