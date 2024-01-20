# Thermal Image processing to detect water bodies from the varying environments
## Sequence for Understanding the Files: (file name with description)

1. thermal_signatures: contains SSAE training with MSE loss, binary cross-entropy, and categorical cross-entropy out of which MSE works best. The file also contains metrics for checking the accuracy of SSAE namely the Dice coefficient, and IOU. Calinski-Harabasz Index and Davies-Bouldin Index
2. mse_clusters: contains the clusters formed after T-SNE on the encoded features from SSAE with MSE loss
3. ssae_focal: contains SSAE training with focal loss and the metrics for it
4. Tsne: contains clustering algorithms namely k-means, GMM, and DBSCAN, it also contains T-SNE plots with image embeddings for the clusters obtained from SSAE with MSE and focal loss along with the intrinsic metrics to check the quality of clusters namely Silhouette score, Calinski-Harabasz Index, and Davies-Bouldin Index
5. ssae_focal_trversky: contains SSAE training with focal tversky loss and metrics for it

## Inferences:
It can be noted that SSAE with MSE and focal loss gave better results on Dice Coefficient. Also, k-means and GMM gave similar clustering results and good clusters
