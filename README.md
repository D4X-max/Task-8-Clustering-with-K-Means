# Task-8-Clustering-with-K-Means


# 1. Loading and Visualizing the Dataset (PCA for 2D View)
I began by loading the dataset using pandas.

I selected the relevant numerical features: Age, Annual Income, and Spending Score.

I standardized these features to ensure they were on the same scale.

I applied Principal Component Analysis (PCA) to reduce the data to two dimensions for visualization.

I plotted the PCA-transformed data to observe any natural groupings or patterns among customers.

# 2. Fitting K-Means and Assigning Cluster Labels
I applied the K-Means clustering algorithm to the standardized dataset.

I initially set the number of clusters (K) to 5, based on common practice for this type of data.

The algorithm assigned a cluster label to each customer, segmenting them into groups.

I appended these cluster labels as a new column in the original dataset for further analysis.

# 3. Determining the Optimal Number of Clusters with the Elbow Method
I ran K-Means clustering for a range of K values (from 1 to 10).

For each K, I calculated the inertia (within-cluster sum of squares).

I plotted the inertia values against the number of clusters to create an Elbow plot.

I identified the “elbow point,” where the rate of decrease in inertia slowed significantly.

This analysis indicated that K=5 was an appropriate choice for the number of clusters.

# 4. Visualizing Clusters with Color-Coding
I visualized the clusters in the 2D PCA space, assigning a unique color to each cluster.

This color-coding allowed me to easily distinguish between different customer segments.

The visualization helped me assess the separation and overlap between clusters.

# 5. Evaluating Clustering Using the Silhouette Score
I calculated the Silhouette Score to evaluate the quality of the clustering.

This score measured how similar each customer was to its own cluster compared to other clusters.

A score of approximately 0.44 indicated a moderate level of cluster separation.

This result suggested that the clustering captured meaningful distinctions among the customer groups.
