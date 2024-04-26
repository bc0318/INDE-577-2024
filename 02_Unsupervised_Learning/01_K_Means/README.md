# K-Means

## Introduction

K-means is one of the most popular and straightforward clustering algorithms in machine learning. It is an **unsupervised learning algorithm** that is used to group data into a predefined number of clusters, where each data point belongs to the cluster with the nearest mean. The algorithm is highly suited for clustering large volumes of data and is widely used in market segmentation, document clustering, image segmentation, and many other applications.

---

## Algorithm

<p align="center">
    <img src="kmeans.png" width = 800 height = 400>
</p>

K-means works as follows:

1. **Initialization:** The process begins by selecting *k* initial centroids, where *k* is the desired number of clusters. The initial centroids are usually chosen randomly from the dataset, although there are more sophisticated methods to initialize centroids that can potentially improve the algorithm's convergence and output.

2. **Assignment:** The algorithm assigns each data point to the nearest centroid, where *nearest* might be defined using Euclidean distance, Manhattan distance, or other metrics depending on the nature of the data. As a result, each iteration forms *k* clusters with associated data points.

3. **Update:** After all points have been assigned to clusters, the centroids of the clusters are recalculated. This is typically done by taking the mean of all points assigned to each cluster.

4. **Iteration:** Step 2 and 3 are repeated until the centroids no longer move significantly or the assignments no long change. This indicates that the algorithm has converged.

---

## Advantages and Disadvantages

Advantages:
- K-means is relatively simple and can be very efficient in terms of computational cost, especially with large datasets
- There are very few parameters to adjust, making k-means easier to set up compared to more complex clustering algorithms

Disadvantages:
- The final clusters can vary significantly based on the initial choice of centroids
- Outliers can skew the centroids, leading to less accurate clusters
- K-means assumes that clusters are spherical and evenly sized, which might not always be the case