# Fundamentals of Data Science Weekk 9 Forum
## Unsupervised Machine Learning
### Ostein Vittorio Vellim
### 2602206783

#### Dataset used: Scikit Wine
#### Evaluation methods used: 
- Silhouette score
- Davies-Bouldin Index
- Agglomerative Clustering
- Spectral Clustering

#### KMeans Clustering
KMeans clustering is a method of partitioning that divides the dataset into K number of clusters. It works by first randomly placing K centroids in the data space, and then data points that are closest to a centroid will be assigned to the centroid. The centroids will then be recalculated based ont he points in each cluster  and will repeat until the centroids no longer change significantly, thus forming clusters.

##### Results for KMeans Clustering
- Silhouette Score:  0.5711381937868838
- Davies-Bouldin Index:  0.5342431775436286
- Rand Score:  0.37111371823084754
- Calinski and Harabasz Score:  561.815657860671


#### MeanShift Clustering
MeanShift clustering is a partitioning algorithm forms clusters out of dense areas in the data space. Each data point are first assigned a window (bandwidth). The window's centers shift to the mean of the points within it, repeating until convergence in the densest areas. This algorithm is quite adaptive as you don't have to specify the number of clusters present.

##### Results for MeanShift Clustering
- Silhouette Score:  0.5024921259394886
- Davies-Bouldin Index:  0.5561495856687338
- Rand Score:  0.39723664098601413
- Calinski and Harabasz Score:  454.0589434652176


#### Agglomerative Clustering
Agglomerative Clustering is a clustering method which uses hierarchy in order to merge data points into clusters. It starts by considering each data point as its own cluster before iteratively merging the closest points. The algortihm stops once a certain number of clusters is reached or when a certain threshold is completed.

##### Results for Agglomerative Clustering
- Silhouette Score:  0.5644796401732068
- Davies-Bouldin Index:  0.5357343073560251
- Rand Score:  0.36840191587483156
- Calinski and Harabasz Score:  552.851711505718


#### Spectral Clustering
Spectral Clustering utilizes eigenvalues of a similarity matrix to perform clustering. It will first construct a similarity matrix from the data. Then the eigenvalues and eigenvectors will be calculated and used to form a new matrix one dimension lower, after which other clustering algorithms can be applied to perform clustering.

##### Results for Spectral Clustering
- Silhouette Score:  0.28034808703238107
- Davies-Bouldin Index:  0.44772255236450287
- Rand Score:  0.000351000351000351
- Calinski and Harabasz Score:  3.3691025466629982


#### Findings

###### Silhoutte Score from Best to Worst
KMeans --> Agglomerative --> MeanShift --> Spectral

###### Davies-Bouldin Index from Best to Wrost
Spectral --> KMeans --> Agglomerative --> Meanshift

###### Rand Score from Best to Worst
MeanShift --> KMeans --> Agglomerative --> Spectral

###### Calinski and Harabasz Score from Best to Worst
KMeans --> Agglomerative --> MeanShift --> Spectral

