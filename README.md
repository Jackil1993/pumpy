This script is written to conduct a case-study reported in the paper "Unsupervised learning-based SKU segmentation" [1].
The script utilizes a free machine learning library “scikit-learn” as a core complementing it with several algorithms.
The concept of data-pipeline is used to consequentially perform the following procedures:
1) to impute the missing data with nearest-neighbour-imputation
2) to standardize the data
3) to identify and trim outliers and small 'blobs' with LOF and mean-shift
4) to cluster the data with k-mean and DBSCAN
5) to improve the eventual clustering result via PCA
Since the ground truth is not provided, the clustering is validated only by internal evaluation, namely by silhouette index, Calinski-Harabazs index and Dunn-index

References:

[1] Jackson, I., Avdeikins, A. and Tolujevs, J., 2018, October. Unsupervised Learning-Based Stock Keeping Units Segmentation.
In International Conference on Reliability and Statistics in Transportation and Communication (pp. 603-612). Springer, Cham.
