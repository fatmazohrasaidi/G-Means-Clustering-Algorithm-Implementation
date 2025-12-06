# G-Means Clustering Algorithm Implementation

## Overview
This project implements the **G-Means clustering algorithm**, an adaptive version of K-Means that automatically determines the optimal number of clusters.
The algorithm uses PCA for dimensionality reduction, Anderson–Darling tests for Gaussian validation, and silhouette scores to evaluate splits.

Two versions are implemented:  
1. **Basic G-Means** with silhouette constraint  
2. **Enhanced G-Means** with centroid initialization as described in the original paper  

## Algorithm Steps  
1. **Dimensionality Reduction** using PCA  
2. **Initialize** with one cluster (global mean)  
3. **Iteratively split clusters** if they are not Gaussian-distributed  
4. **Validate splits** using silhouette score and minimum centroid distance  
5. **Stop** when no valid splits remain or max clusters reached  

## Datasets Used  
- Iris  
- Digits  
- Wine  
- Breast Cancer  
- Synthetic Blobs, Moons, and Circles  

## Evaluation  
- **Similarity Score**: Compares predicted vs. true cluster count  
- **Visualization**: Bar charts comparing true vs. predicted k  
- **Iteration Tracking**: Measures convergence speed  

## Technologies  
- Python 3  
- NumPy, scikit-learn, SciPy  
- Matplotlib for visualization  
- Jupyter Notebook for interactive analysis  
