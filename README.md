# Clustering Analysis Using the Lenses Dataset

Results Table:


<img width="581" alt="image" src="https://github.com/user-attachments/assets/a586edce-7a1c-40b5-b4f8-8e5b2d79dbe4">

Note: The table shows the performance of K-Means clustering using different pre-processing techniques and the number of clusters ranging from 3 to 5.


Graphs:

Elbow Method for Optimal Clusters (K-Means)

The elbow plot suggests that the optimal number of clusters is 4 for the K-Means and hierarchical clustering algorithms. This is based on the point where the rate of decrease in the distortion slows down significantly.

![image](https://github.com/user-attachments/assets/648d5036-1678-465f-9ce4-f21372abe826)

![image](https://github.com/user-attachments/assets/6e47bea7-be71-42d7-9c84-bfa962042f2e)


Silhouette Analysis for Clustering Performance

Silhouette scores indicate how well each object is clustered. Higher scores suggest that the data is well-clustered, with most points lying within their own cluster.


K-Means Shift Distribution Plot

This plot shows the distribution of data points across different clusters using the K-Means shift algorithm. It appears that the results are not as informative as the K-Means or hierarchical clustering.

![newplot](https://github.com/user-attachments/assets/98947397-607a-4ed9-9999-30745f190065)


Conclusion
Based on the results table and visualizations, the following conclusions can be drawn:

Optimal Number of Clusters: The elbow plot indicates that the optimal number of clusters for the lenses dataset is 4 for both K-Means and hierarchical clustering. This is consistent with the Silhouette scores, which are higher for 4 clusters compared to 3 or 5.

Effectiveness of Different Clustering Techniques: The K-Means and hierarchical clustering algorithms perform well with this dataset, showing distinguishable clusters. On the other hand, the K-Means shift algorithm does not yield meaningful results for this dataset.

Pre-processing Impact on Performance: Various pre-processing steps, such as normalization, transformation, and principal component analysis (PCA), were applied to observe their effects on clustering performance:

Normalization and Transformation generally improved the Silhouette score and Calinski-Harabasz index, indicating better-defined clusters.
PCA (Principal Component Analysis) had mixed results, with some degradation in clustering quality compared to other techniques.
Combined Pre-processing (T+N, T+N+PCA) showed a more consistent performance but did not always outperform simpler methods.
Performance Metrics Used: The following metrics were used to evaluate the clustering quality:

Silhouette Score: Measures how similar a point is to its own cluster compared to other clusters.
Calinski-Harabasz Index: Evaluates the ratio of the sum of between-cluster dispersion to within-cluster dispersion.
Davies-Bouldin Index: Measures the average similarity ratio of each cluster with the cluster most similar to it; lower values are preferable.
In conclusion, the clustering analysis suggests that the K-Means and hierarchical clustering approaches, with a cluster count of 4, are suitable for the lenses dataset. Various pre-processing methods can slightly improve the results, but the choice of the number of clusters has the most significant impact on clustering quality.





