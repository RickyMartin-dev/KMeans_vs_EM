# KMeans_vs_EM

In this notebook we will be implementing both K-means clustering and EM Algorithm on 2D points. Both of these algorithms are methods to divide the given set of points into k clusters (groups), such that all points in a cluster are "close together". The number k is chosen in advance manually and is not computed by the algorithms.

The main difference between the two algorithms is that K-means is a "hard clustering" method, whereas EM is used to create a "soft clustering". This means that in K-means, each point is either 100% in a cluster, or not in it. Whereas in EM Algorithm, we compute a (Gaussian) probability distribution for each cluster. We can use these to compute the probability for a point to be in a cluster, for all pairs of points and clusters. So for each point, we find the probability that it is in each of the clusters.
