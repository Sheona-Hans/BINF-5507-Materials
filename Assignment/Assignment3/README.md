# Clustering Algorithms Comparison: DBSCAN, K-Means, and Hierarchical Clustering
This repository demonstrates and compares three popular clustering algorithms: DBSCAN, K-Means, and Hierarchical Clustering, using a synthetic 2D dataset. The comparison is based on their performance in clustering non-linearly separable data generated with the make_moons dataset from scikit-learn. <br>
<br>
### Introduction
Clustering is an unsupervised machine learning technique that involves grouping similar data points together. This repository implements and visualizes the clustering results of three well-known algorithms: <br>
<br>
DBSCAN (Density-Based Spatial Clustering of Applications with Noise)<br>
K-Means (Partitioning-based clustering)<br>
Hierarchical Clustering (Agglomerative hierarchical clustering)<br>
<br>
The dataset used for clustering is generated using the make_moons function from scikit-learn, which creates a two-class synthetic dataset with a crescent moon shape. This dataset is non-linearly separable, making it an interesting test case for clustering algorithms.<br>
<br>

### DBSCAN
DBSCAN (Density-Based Spatial Clustering of Applications with Noise) is a density-based clustering algorithm that identifies clusters based on the density of points in a region. It requires two parameters:<br>
eps (epsilon): The maximum distance between two points to be considered neighbors.<br>
min_samples: The minimum number of points required to form a dense region (core point).<br>
DBSCAN can detect arbitrarily shaped clusters and also identifies outliers (points that do not belong to any cluster).<br>
<br>
### K-Means
K-Means is a centroid-based clustering algorithm that partitions data into k clusters, minimizing the variance within each cluster. It requires the number of clusters (k) to be specified beforehand. K-Means assumes that clusters are spherical and have similar sizes, making it less suitable for datasets with complex shapes.<br>
<br>
### Hierarchical Clustering
Hierarchical Clustering builds a hierarchy of clusters using a bottom-up (agglomerative) or top-down (divisive) approach. In this implementation, the agglomerative method is used, where each point starts as its own cluster, and clusters are merged iteratively based on a distance metric (Ward's method in this case). The result is a dendrogram, which shows the hierarchical relationship between the clusters.<br>
<br>
## How to run<br>
Prerequisites<br>
Before running the code, make sure you have the following Python libraries installed:<br>
<br>
1. numpy
2. matplotlib
3. scikit-learn
4. scipy

## How to run
Open the notebook
Filename: main.ipynb
Execute each cell of the notebook sequentially until the comparison and visualization cells

