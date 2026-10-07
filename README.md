# Bank Customer Segmentation

This project applies **Data Mining and Unsupervised Learning techniques** to analyze and segment bank customers based on selected economic indicators.

## Project Objective

The main objective of this project is to identify meaningful customer groups using clustering techniques and analyze their relationship with customer subscription behavior.

## Dataset

The project uses the dataset:

`bank-customers.csv`

## Features Used for Clustering

The clustering analysis is based on the following features:

- `emp.var.rate`
- `euribor3m`
- `nr.employed`
- `cons.conf.idx`

## Project Workflow

The project currently includes:

- Data exploration
- Missing value checking
- Factor Analysis
- KMO Test
- Bartlett's Test of Sphericity
- Feature selection
- Feature scaling using StandardScaler
- Hopkins Statistic for clustering tendency
- K-Means Clustering
- DBSCAN Clustering
- Elbow Method
- Silhouette Score
- Calinski-Harabasz Score
- Davies-Bouldin Index
- PCA for dimensionality reduction
- Cluster visualization using Plotly
- Comparison between K-Means and DBSCAN
- Analysis of clusters against customer subscription behavior

## Machine Learning Techniques

### K-Means

K-Means clustering is applied to divide the dataset into customer groups based on similarities between the selected features.

Different values of K are evaluated using:

- Elbow Method
- Silhouette Score
- Calinski-Harabasz Index

### DBSCAN

DBSCAN is also applied to identify clusters and detect noise points without requiring the number of clusters to be specified in advance.

Current parameters:

```python
eps = 0.5
min_samples = 15