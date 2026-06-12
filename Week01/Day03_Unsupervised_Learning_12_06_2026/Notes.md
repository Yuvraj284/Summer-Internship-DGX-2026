# Day 03 – Unsupervised Learning and Clustering

## Introduction to Unsupervised Learning

Machine Learning algorithms are broadly divided into two categories: Supervised Learning and Unsupervised Learning.

In Supervised Learning, the dataset contains both input features and corresponding output labels. The model learns from these labeled examples and predicts outputs for new data.

In Unsupervised Learning, the dataset contains only input features and no target labels. The objective is to discover hidden patterns, relationships, or structures within the data.

Unsupervised Learning is commonly used for:

* Clustering
* Customer Segmentation
* Pattern Recognition
* Anomaly Detection
* Data Exploration

---

## Clustering

Clustering is a technique used to group similar data points together. Data points within the same cluster are more similar to each other than to those in other clusters.

For example, a company may group customers based on purchasing behavior without having predefined categories.

Some commonly used clustering algorithms are:

* K-Means Clustering
* Hierarchical Clustering
* DBSCAN

---

# K-Means Clustering

K-Means is one of the most widely used clustering algorithms.

The main objective of K-Means is to divide the dataset into K distinct clusters based on similarity.

### Working of K-Means

1. Choose the number of clusters (K).
2. Randomly initialize K centroids.
3. Assign each data point to the nearest centroid.
4. Recalculate the centroid of each cluster.
5. Repeat the process until the centroids stop changing significantly.

### Centroid

A centroid represents the center of a cluster. During each iteration, K-Means updates the centroid position to improve clustering.

### Advantages

* Easy to understand and implement.
* Fast and efficient on large datasets.
* Works well when clusters are clearly separated.

### Disadvantages

* The value of K must be specified beforehand.
* Sensitive to outliers and noise.
* May not perform well for irregularly shaped clusters.

---

## Elbow Method

Choosing the correct value of K is an important challenge in K-Means.

The Elbow Method helps determine the optimal number of clusters by plotting the Within Cluster Sum of Squares (WCSS) against different values of K.

The point where the graph starts bending like an elbow is considered the best value of K.

---

# Hierarchical Clustering

Hierarchical Clustering builds a hierarchy of clusters instead of creating a fixed number of clusters.

The algorithm starts by treating each data point as an individual cluster and gradually merges similar clusters until all points belong to a single cluster.

### Types of Hierarchical Clustering

1. Agglomerative Clustering (Bottom-Up)
2. Divisive Clustering (Top-Down)

Agglomerative clustering is the most commonly used approach.

### Dendrogram

A dendrogram is a tree-like diagram used to visualize hierarchical clustering.

It helps understand how clusters are formed and can be used to decide the number of clusters.

### Advantages

* No need to specify the number of clusters initially.
* Easy visualization using dendrograms.
* Useful for understanding relationships between clusters.

### Disadvantages

* Computationally expensive for large datasets.
* Difficult to modify once clusters are merged.

---

# DBSCAN

DBSCAN stands for:

Density-Based Spatial Clustering of Applications with Noise

It is a density-based clustering algorithm that groups together points located in dense regions and identifies points in sparse regions as noise.

Unlike K-Means, DBSCAN does not require specifying the number of clusters beforehand.

### Important Parameters

### Epsilon (ε)

Defines the radius around a point for searching neighboring points.

### MinPts

Represents the minimum number of points required to form a dense region.

### Working of DBSCAN

1. Select a point.
2. Find neighboring points within the epsilon radius.
3. If enough neighbors exist, create a cluster.
4. Expand the cluster by including connected dense regions.
5. Points that do not belong to any cluster are treated as noise.

### Advantages

* No need to specify the number of clusters.
* Detects outliers automatically.
* Works well for irregularly shaped clusters.

### Disadvantages

* Sensitive to parameter selection.
* Performance may decrease when cluster densities vary significantly.

---

# Outliers and Noise

### Outlier

An outlier is a data point that is significantly different from the majority of the dataset.

Example:

If most student marks are between 60 and 90, a mark of 5 or 100 may be considered an outlier.

### Noise

Noise refers to random, irrelevant, or meaningless data that does not follow any clear pattern.

DBSCAN is particularly effective at identifying noise points.

---

# Comparison of Clustering Algorithms

| Feature                            | K-Means | Hierarchical | DBSCAN    |
| ---------------------------------- | ------- | ------------ | --------- |
| Need to specify number of clusters | Yes     | No           | No        |
| Handles noise                      | Poor    | Moderate     | Excellent |
| Supports irregular cluster shapes  | No      | Limited      | Yes       |
| Uses centroids                     | Yes     | No           | No        |
| Dendrogram support                 | No      | Yes          | No        |
| Suitable for large datasets        | Yes     | Moderate     | Moderate  |

---

# Conclusion

Unsupervised Learning focuses on discovering hidden structures and patterns in data without using labeled outputs. Clustering is one of the most important applications of Unsupervised Learning.

K-Means, Hierarchical Clustering, and DBSCAN are three widely used clustering algorithms, each having its own strengths and limitations. Understanding these algorithms helps in organizing data, identifying patterns, and performing exploratory analysis on real-world datasets.