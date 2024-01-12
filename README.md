# k_means_clustering
Applying k-means on gene expression data.


This repository contains code for analyzing gene expression data from 62 different individuals, focusing on the application of k-means clustering for patient categorization. The dataset includes gene expression information from 2000 different genes, with the first 40 rows representing individuals with colon cancer, the next 21 rows from healthy individuals, and the last row from a patient with an unknown health status.

This repository presents a detailed analysis of gene expression data, specifically focusing on the application of k-means clustering for patient categorization. The provided Python code executes a series of tasks, starting with the loading of the gene expression data from the gene_expression_matrix.txt file using numpy.loadtxt. The resulting matrix is a 62 x 2000 array of floating-point numbers, representing gene expression values for 62 individuals across 2000 genes. The first three columns of this matrix are printed for initial inspection.

Subsequently, the data is standardized for k-means clustering by subtracting the mean of each dimension and dividing by its standard deviation across all observations. The first three columns of the standardized matrix are printed to showcase the transformation. The k-means clustering algorithm is then implemented using cosine similarity as the distance metric, with the objective of clustering the 62 patients into 2 clusters labeled 0 and 1.

To enhance the robustness of the clustering, the k-means algorithm is run five times with different initial centroids, and the squared error distortion is calculated and reported for each solution. In the subsequent analysis, the clustering solution with the lowest squared error distortion is examined. This includes calculating the percentage of cancer patients in each of the two clusters, excluding the 62nd patient, and printing the cluster assignment for the 62nd patient.

Finally, the conclusion section prompts a thorough analysis of the results, emphasizing whether there are significant differences between the clusters in terms of the percentage of cancer patients. The discussion encourages contemplating the reliability of determining the cancer status of the 62nd patient based on the clustering outcomes. In essence, this repository offers a comprehensive exploration of gene expression data through k-means clustering, providing valuable insights into potential patterns associated with different health statuses.
