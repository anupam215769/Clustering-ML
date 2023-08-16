# Clustering

Clustering or cluster analysis is a machine learning technique, which groups the unlabelled dataset. It can be defined as **"A way of grouping the data points into different clusters, consisting of similar data points. The objects with the possible similarities remain in a group that has less or no similarities with another group."**

It does it by finding some similar patterns in the unlabelled dataset such as shape, size, color, behavior, etc., and divides them as per the presence and absence of those similar patterns.

It is an [Unsupervised learning](https://en.wikipedia.org/wiki/Unsupervised_learning) method, hence no supervision is provided to the algorithm, and it deals with the unlabeled dataset.

After applying this clustering technique, each cluster or group is provided with a cluster-ID. ML system can use this id to simplify the processing of large and complex datasets.

### K-Means Clustering [Code](https://github.com/anupam215769/Clustering-ML/blob/main/K-Means%20Clustering/k_means_clustering.ipynb) OR <a href="https://colab.research.google.com/github/anupam215769/Clustering-ML/blob/main/K-Means%20Clustering/k_means_clustering.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>

### Hierarchical Clustering [Code](https://github.com/anupam215769/Clustering-ML/blob/main/Hierarchical%20Clustering/hierarchical_clustering.ipynb) OR <a href="https://colab.research.google.com/github/anupam215769/Clustering-ML/blob/main/Hierarchical%20Clustering/hierarchical_clustering.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>

> Don't forget to add Required Data files in colab. Otherwise it won't work.


## K-Means Clustering

K-Means Clustering is an unsupervised learning algorithm that is used to solve the clustering problems in machine learning or data science. In this topic, we will learn what is K-means clustering algorithm, how the algorithm works, along with the Python implementation of k-means clustering.

It is a centroid-based algorithm, where each cluster is associated with a centroid. The main aim of this algorithm is to minimize the sum of distances between the data point and their corresponding clusters.
The algorithm takes the unlabeled dataset as input, divides the dataset into k-number of clusters, and repeats the process until it does not find the best clusters. The value of k should be predetermined in this algorithm.

![kmeans](https://i.imgur.com/9l2R8Ck.png)

### Random Initialization Trap in K-Means

Random initialization trap is a problem that occurs in the K-means algorithm. In random initialization trap when the centroids of the clusters to be generated are explicitly defined by the User then inconsistency may be created and this may sometimes lead to generating wrong clusters in the dataset. So random initialization trap may sometimes prevent us from developing the correct clusters. 

![trap](https://i.imgur.com/UNvqxTw.jpg)


### Elbow Method To Find K Number Of Clusters

The Elbow method is one of the most popular ways to find the optimal number of clusters. This method uses the concept of WCSS value. **WCSS** stands for **Within Cluster Sum of Squares**, which defines the total variations within a cluster. The formula to calculate the value of WCSS (for 3 clusters) is given below:

![wcss](https://i.imgur.com/T2eyDAy.png)

Since the graph shows the sharp bend, which looks like an elbow, hence it is known as the elbow method. The graph for the elbow method looks like the below image:

![method](https://i.imgur.com/i78nH4n.png)


## Hierarchical Clustering

Hierarchical clustering is another unsupervised machine learning algorithm, which is used to group the unlabeled datasets into a cluster and also known as **hierarchical cluster analysis** or **HCA**.

In this algorithm, we develop the hierarchy of clusters in the form of a tree, and this tree-shaped structure is known as the **dendrogram**.

Sometimes the results of K-means clustering and hierarchical clustering may look similar, but they both differ depending on how they work. As there is no requirement to predetermine the number of clusters as we did in the K-Means algorithm.

![h](https://i.imgur.com/WNlHV9I.png)

The hierarchical clustering technique has two approaches:

- **Agglomerative:** Agglomerative is a bottom-up approach, in which the algorithm starts with taking all data points as single clusters and merging them until one cluster is left.

- **Divisive:** Divisive algorithm is the reverse of the agglomerative algorithm as it is a top-down approach.

### Measure for the distance between two clusters

![i](https://i.imgur.com/tLIbjQi.png)


### Woking of Dendrogram in Hierarchical clustering

The dendrogram is a tree-like structure that is mainly used to store each step as a memory that the HC algorithm performs. In the dendrogram plot, the Y-axis shows the Euclidean distances between the data points, and the x-axis shows all the data points of the given dataset.

![f](https://i.imgur.com/u9h18GM.jpg)

In the above diagram, the left part is showing how clusters are created in agglomerative clustering, and the right part is showing the corresponding dendrogram.

- As we have discussed above, firstly, the datapoints P2 and P3 combine together and form a cluster, correspondingly a dendrogram is created, which connects P2 and P3 with a rectangular shape. The hight is decided according to the Euclidean distance between the data points.

- In the next step, P5 and P6 form a cluster, and the corresponding dendrogram is created. It is higher than of previous, as the Euclidean distance between P5 and P6 is a little bit greater than the P2 and P3.

- Again, two new dendrograms are created that combine P1, P2, and P3 in one dendrogram, and P4, P5, and P6, in another dendrogram.

- At last, the final dendrogram is created that combines all the data points together.


## Comparison

| Clustering Model        | Pros                                                                                                            | Cons                                  |
|-------------------------|-----------------------------------------------------------------------------------------------------------------|---------------------------------------|
| K-Means                 | Simple to understand, easily adaptable, works well on small or large datasets, fast, efficient and performance  | Need to choose the number of clusters |
| Hierarchical Clustering | The optimal number of clusters can be obtained by the model itself, practical visualisation with the dendrogram | Not appropriate for large datasets    |


## Related Repositories

### [Data Preprocessing](https://github.com/anupam215769/Data-Preprocessing-ML)

### [Regression](https://github.com/anupam215769/Regression-ML)

### [Classification](https://github.com/anupam215769/Classification-ML)

### [Association Rule Learning](https://github.com/anupam215769/Association-Rule-Learning-ML)

### [Reinforcement Learning](https://github.com/anupam215769/Reinforcement-Learning-ML)


