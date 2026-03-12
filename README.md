# Machine Learning Models: Clustering, Regression and Classification

This project contains implementations of several machine learning algorithms applied to different types of problems:

- Unsupervised learning (clustering)
- Regression
- Classification

The goal of this project is to compare different ML approaches and evaluate their performance on well-known datasets.

## Project Structure

project/
│
├── notebooks/
│   ├── iris_clustering.ipynb
│   ├── boston_regression.ipynb
│   ├── mnist_classification.ipynb
│
├── data/
│
├── README.md
│
└── requirements.txt


## Datasets Used

### IRIS Dataset (Clustering)

The IRIS dataset contains information about three species of iris flowers:
- Iris Setosa
- Iris Versicolor
- Iris Virginica

Each observation contains:

- Sepal length
- Sepal width
- Petal length
- Petal width

The goal was to cluster the flowers based on their features.

Algorithms used:

- K-Means
- DBSCAN
- Agglomerative Clustering

Key findings:

- K-Means successfully identified 3 clusters
- Agglomerative clustering also performed well
- DBSCAN required more parameter tuning

## Boston Housing Dataset (Regression)

This dataset contains housing data from Boston.

Goal:
Predict housing prices using regression models.

Models used:

- Random Forest
- Gradient Boosting

Evaluation metrics:

- RMSE
- R² score

Results:

Random Forest:
- RMSE ≈ 0.5089
- R² ≈ 0.75

Gradient Boosting:
- R² ≈ 0.82
- RMSE ≈ 1.42

Conclusion:

- Random Forest produced lower error
- Gradient Boosting explained more variance

## MNIST Dataset (Classification)

MNIST is a dataset of handwritten digits (0–9).

Goal:
Classify digits using different ML models.

Models used:

- Logistic Regression
- Random Forest
- K-Nearest Neighbours (KNN)

Results:

Logistic Regression:
- Accuracy improved from 0.89 to 0.93 after normalization

Random Forest:
- Accuracy ≈ 0.9399

KNN:
- Highest accuracy among tested models

Conclusion:

KNN showed the best performance but requires more computational resources.

## Technologies Used

Python

Libraries:

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
