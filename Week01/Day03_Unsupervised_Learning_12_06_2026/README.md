# Day 03 - Unsupervised Learning and Clustering

## Objective

The objective of this activity was to understand the fundamentals of Unsupervised Learning and implement different clustering algorithms to discover hidden patterns in data.

Unlike supervised learning, unsupervised learning works with unlabeled data and attempts to group similar observations based on their characteristics.

---

## Topics Covered

- Introduction to Unsupervised Learning
- Clustering
- K-Means Clustering
- Elbow Method
- Hierarchical Clustering
- Dendrogram
- DBSCAN
- Noise and Outlier Detection
- Cluster Analysis and Interpretation

---

## Dataset Used

### Country Development Dataset

The dataset contains socioeconomic and health-related indicators for 167 countries.

### Features

- Child Mortality Rate
- Exports
- Health Expenditure
- Imports
- Income
- Inflation
- Life Expectancy
- Total Fertility Rate
- GDP per Capita

### Additional File

- `data-dictionary.csv` was used to understand the meaning of each feature in the dataset.

---

## Why This Dataset?

The dataset does not contain predefined labels or target variables, making it suitable for unsupervised learning.

The objective was to identify natural groupings of countries based on their economic, health, and demographic indicators.

---

# 1. K-Means Clustering

K-Means Clustering was applied after standardizing all numerical features.

### Steps Performed

1. Data Loading and Inspection
2. Feature Scaling using StandardScaler
3. Elbow Method for selecting optimal K
4. Model Training
5. Cluster Assignment
6. Cluster Analysis

### Results

The Elbow Method suggested:

K = 3

The algorithm grouped countries into three major clusters that broadly represented:

- Developed Countries
- Developing Countries
- Underdeveloped Countries

### Key Learning

K-Means is simple, efficient, and effective when the number of clusters is known beforehand.

---

# 2. Hierarchical Clustering

Hierarchical Clustering was implemented using Agglomerative Clustering.

### Steps Performed

1. Data Standardization
2. Dendrogram Construction
3. Cluster Selection
4. Agglomerative Clustering
5. Cluster Interpretation

### Results

The dendrogram indicated that three clusters were appropriate for the dataset.

Countries with similar socioeconomic characteristics were grouped together, producing results similar to K-Means.

### Key Learning

Hierarchical Clustering provides a visual representation of cluster formation through a dendrogram and does not require selecting the number of clusters initially.

---

# 3. DBSCAN

DBSCAN (Density-Based Spatial Clustering of Applications with Noise) was implemented to identify clusters based on data density.

### Steps Performed

1. Data Standardization
2. Parameter Selection (`eps` and `min_samples`)
3. Density-Based Clustering
4. Noise Detection
5. Cluster Analysis

### Results

| Cluster | Number of Countries |
|----------|----------|
| Cluster 0 | 21 |
| Cluster 1 | 75 |
| Cluster 2 | 18 |
| Noise (-1) | 53 |

### Key Learning

Unlike K-Means and Hierarchical Clustering, DBSCAN automatically identified countries that did not strongly belong to any cluster and marked them as noise points.

---

## Comparison of Algorithms

| Feature | K-Means | Hierarchical | DBSCAN |
|----------|----------|----------|----------|
| Requires Number of Clusters | Yes | No | No |
| Uses Centroids | Yes | No | No |
| Dendrogram Support | No | Yes | No |
| Detects Noise | No | No | Yes |
| Handles Outliers | Poor | Moderate | Excellent |

---

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- SciPy

---

## Files Included

- Notes.md
- Country-data.csv
- data-dictionary.csv
- KMeans_Country_Data.ipynb
- Hierarchical_Country_Data.ipynb
- DBSCAN_Country_Data.ipynb
- README.md

---

## Learning Outcomes

After completing this activity, I learned:

- The difference between supervised and unsupervised learning.
- How clustering algorithms identify hidden patterns in data.
- How K-Means uses centroids for clustering.
- How Hierarchical Clustering builds a hierarchy of clusters.
- How DBSCAN detects both clusters and outliers.
- The importance of feature scaling in clustering problems.
- How different clustering algorithms can produce different insights from the same dataset.

---

## Conclusion

This activity provided practical experience with three important clustering algorithms: K-Means, Hierarchical Clustering, and DBSCAN. By applying all three techniques to the same country dataset, it was possible to compare their behavior, strengths, and limitations. The exercise demonstrated how unsupervised learning can reveal meaningful patterns and group similar countries without requiring predefined labels.