# Credit Card Customer Segmentation

## Project Description
The primary business objective of this project is to segment a bank's credit card customer base into distinct clusters based on their financial behaviors. Identifying specific customer profiles enables better tailoring of marketing campaigns and more effective credit risk management. The dataset used contains extensive behavioral information, such as balances, purchases, cash advances, and payment histories. This task was accomplished using unsupervised machine learning techniques.

## Technologies Used
* **Python**
* **Pandas & NumPy:** Data manipulation and calculation.
* **Scikit-learn:** 
    * Preprocessing: `MinMaxScaler`, `StandardScaler`, `RobustScaler`.
    * Distances: `euclidean_distances`, `manhattan_distances`, `cosine_similarity`.
    * Clustering Algorithms: `KMeans`, `AgglomerativeClustering`, `DBSCAN`.
    * Evaluation: `silhouette_score`, `davies_bouldin_score`.
    * Dimensionality Reduction: `PCA`, `TSNE`.
* **SciPy:** `zscore`, `mahalanobis`, `linkage`, `dendrogram`.
* **UMAP:** Advanced dimensionality reduction and visualization.
* **Seaborn & Matplotlib:** Heatmaps, distributions, and cluster visualizations.

## Methodology
The analytical workflow is structured as follows:
1. **Exploratory Data Analysis & Cleaning:** Handling missing values in features like `MINIMUM_PAYMENTS` and `CREDIT_LIMIT` using median imputation to preserve distributions. Irrelevant features (e.g., `CUST_ID`) were dropped.
2. **Outlier Analysis & Transformation:** Financial data is highly skewed with numerous outliers. The project analyzed these using Interquartile Range (IQR) and boxplots, and addressed them to stabilize the clustering algorithms.
3. **Clustering & Evaluation:** Applying various unsupervised algorithms (K-Means, Hierarchical Clustering, DBSCAN). The models were evaluated using metrics like Silhouette Score and Davies-Bouldin Index to determine the optimal number of clusters and algorithm fit.
4. **Dimensionality Reduction & Visualization:** Using PCA, t-SNE, and UMAP to reduce the dataset's dimensionality to 2D/3D spaces, allowing for clear visual interpretation of the resulting customer segments.

## File Structure
* `lista3.ipynb` - The Jupyter Notebook containing the full analysis, from EDA to final cluster visualizations.
* `CC GENERAL.csv` - The input dataset containing credit card customer behavioral data.
