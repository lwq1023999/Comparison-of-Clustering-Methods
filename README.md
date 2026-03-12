# Comparison of Clustering Methods

![Python](https://img.shields.io/badge/Python-3.11.3-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Clustering-orange)
![Status](https://img.shields.io/badge/Project-Completed-green)

## Project Overview

This repository contains the implementation and experimental analysis conducted for a postgraduate dissertation completed as part of the MSc in Data Science and Analytics. The project investigates the behaviour and performance of several widely used clustering algorithms across datasets with different structural characteristics.

The research focuses on a comparative evaluation of four clustering methods:

- K-Means  
- DBSCAN  
- Agglomerative Clustering  
- Gaussian Mixture Models (GMM)

These algorithms are applied to multiple datasets, including synthetic data, Spotify audio features, and the MNIST handwritten digit dataset. The objective is to analyse how clustering algorithms perform under varying conditions such as high dimensionality, noise, and overlapping cluster structures.

The study also examines the role of dimensionality reduction techniques, particularly Principal Component Analysis (PCA), in improving clustering performance for high-dimensional data. A variety of internal and external evaluation metrics are used to assess the quality and effectiveness of the clustering results.

The overall goal of this dissertation is to provide a systematic comparison of clustering techniques and highlight the strengths and limitations of each approach when applied to datasets with different characteristics.

---

## Objectives

The main objectives of this research are:

- Compare the performance of different clustering algorithms on datasets with varying complexity.
- Investigate approaches for selecting the optimal number of clusters.
- Analyse how noise and irrelevant features influence clustering performance.
- Evaluate the impact of dimensionality reduction on clustering quality.
- Assess clustering results using both internal and external evaluation metrics.

---

## Clustering Algorithms

### K-Means
K-Means is a partition-based clustering algorithm that groups data points into clusters by minimizing the within-cluster variance.

### DBSCAN
DBSCAN (Density-Based Spatial Clustering of Applications with Noise) is a density-based clustering method that identifies clusters based on regions of high data density and detects noise points.

### Agglomerative Clustering
Agglomerative clustering is a hierarchical clustering technique that builds clusters by iteratively merging the closest clusters based on a chosen linkage criterion.

### Gaussian Mixture Models (GMM)
Gaussian Mixture Models are probabilistic clustering models that assume data is generated from a mixture of Gaussian distributions. GMM allows soft clustering where each data point can belong to multiple clusters with different probabilities.

---

## Datasets

### Synthetic Data
Synthetic datasets were generated to evaluate clustering algorithms in controlled environments where the true cluster structure is known.

### Spotify Dataset
The Spotify dataset contains audio feature information such as danceability, energy, tempo, and acousticness. The dataset was obtained from [Kaggle](https://www.kaggle.com/datasets/zaheenhamidani/ultimate-spotify-tracks-db).

### MNIST Dataset
The MNIST dataset consists of grayscale images of handwritten digits. Each image is represented as a high-dimensional feature vector.

---

## Dimensionality Reduction

Principal Component Analysis (PCA) was applied as a preprocessing step to reduce dataset dimensionality. PCA helps remove redundant features while retaining the most important variance in the data, which improves clustering performance for high-dimensional datasets.

---

## Evaluation Metrics

### Internal Evaluation Metrics

Internal validation metrics evaluate the quality of clustering based solely on considering the
dataset and the clustering output, without the need for external labels.

- Silhouette Score  
- Davies–Bouldin Index  
- Calinski–Harabasz Index  

### External Evaluation Metrics

External validation metrics gauge clustering quality by comparing predicted cluster labels against
the known ground-truth labels.

- Adjusted Rand Index (ARI)  
- Normalized Mutual Information (NMI)

---

## Key Findings

The experimental results highlight several important observations:

- K-Means, Agglomerative Clustering, and GMM generally produced more stable clustering results.
- DBSCAN performed well on lower-dimensional data but struggled with high-dimensional datasets.
- PCA significantly improved clustering performance on the Spotify dataset.
- For the MNIST dataset, GMM achieved stronger alignment with the true labels compared to other algorithms.
- No single clustering algorithm consistently performed best across all datasets.

---

## Technologies Used

The project was implemented using the following tools and libraries:

- Python
- NumPy
- pandas
- scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Repository Structure
