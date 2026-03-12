# Clustering Technique: A Comprehensive Overview

## Overview
This project presents a comparative study of four clustering algorithms:

- K-Means
- DBSCAN
- Agglomerative Clustering
- Gaussian Mixture Models (GMM)

The algorithms are evaluated on three different datasets:

- Synthetic data
- Spotify track features
- MNIST handwritten digits

The aim is to examine how clustering performance changes under different data conditions such as noise, dimensionality, sparsity, and cluster overlap.

## Objectives
The main objectives of this project are:

- Compare the performance of major clustering algorithms on datasets of different complexity
- Investigate how well cluster-number selection methods identify the correct number of clusters
- Evaluate the effect of noise and irrelevant dimensions on clustering stability
- Study the role of dimensionality reduction in high-dimensional datasets
- Assess clustering quality using both internal and external evaluation metrics

## Algorithms Used
### 1. K-Means
A partition-based clustering method that groups data by minimizing within-cluster variance.

### 2. DBSCAN
A density-based clustering method that can detect arbitrarily shaped clusters and identify noise points.

### 3. Agglomerative Clustering
A hierarchical clustering approach that builds a tree of clusters using linkage criteria.

### 4. Gaussian Mixture Model (GMM)
A probabilistic model-based clustering approach that supports soft clustering and elliptical clusters.

## Datasets
### Synthetic Data
Used for controlled experiments where the true number of clusters is known.

### Spotify Dataset
A real-world high-dimensional dataset based on audio track features.

### MNIST Dataset
A high-dimensional image dataset of handwritten digits used to test clustering under sparse and overlapping structure.

## Dimensionality Reduction
Principal Component Analysis (PCA) was applied as a preprocessing step to reduce dimensionality and improve clustering performance, especially on Spotify and MNIST.

## Evaluation Metrics
### Internal Metrics
- Silhouette Score
- Davies–Bouldin Index (DBI)
- Calinski–Harabasz Index (CHI)

### External Metrics
- Adjusted Rand Index (ARI)
- Normalized Mutual Information (NMI)

## Key Findings
- K-Means, Agglomerative Clustering, and GMM generally produced more stable and interpretable results
- DBSCAN was highly sensitive to parameter tuning and struggled in high-dimensional settings
- PCA significantly improved clustering performance on the Spotify dataset
- On MNIST, GMM achieved the best alignment with true digit labels at selected component settings
- No single clustering algorithm performed best across all datasets

## Tech Stack
- Python 3.11
- NumPy
- pandas
- scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Repository Structure
```text
.
├── data/
├── notebooks/
├── src/
├── figures/
├── README.md
└── requirements.txt
