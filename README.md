# Penguin Species Identification using K-Means Clustering

This Jupyter Notebook utilizes a dataset containing penguin measurements to identify groups in the data using K-means clustering. The dataset consists of five columns:

1. **culmen_length_mm:** Culmen length (mm)
2. **culmen_depth_mm:** Culmen depth (mm)
3. **flipper_length_mm:** Flipper length (mm)
4. **body_mass_g:** Body mass (g)
5. **sex:** Penguin sex

Unfortunately, the species of penguin has not been recorded in the dataset. However, we know that there are three species native to the region: Adelie, Chinstrap, and Gentoo. Our task is to identify groups in the dataset using K-means clustering.

## Steps Included in the Notebook:

### 1. Data Preprocessing:

- **Handling Categorical Data:** Convert categorical values in the 'sex' column into dummy variables to include them in the analysis.
- **Data Scaling:** Standardize the numerical features using StandardScaler to ensure that each feature contributes equally to the clustering process.

### 2. Principal Component Analysis (PCA)

- **Finding Optimal Number of Components:** Perform PCA analysis to reduce the dimensionality of the dataset and find the optimal number of components. Select components with eigenvalues greater than 0.1 to retain meaningful variance.

### 3. Determining Optimal Number of Clusters (K)

- **Elbow Method:** Utilize the elbow method to determine the optimal number of clusters (K) for K-means clustering. Plot the within-cluster sum of squares (WCSS) against the number of clusters and identify the elbow point.

### 4. K-Means Clustering

- **Fitting K-Means Model:** Refit the K-means model on the standardized data using the optimal number of clusters obtained from the elbow method.
- **Visualizing Clusters:** Visualize the clusters by plotting the data points with different colors corresponding to their cluster labels.

### 5. Results Interpretation

- **Table of Cluster Labels and Mean Feature Values:** Create a table to display the labels of data points and their corresponding mean values for different features within each cluster. This helps in interpreting the characteristics of each cluster.

## Usage Instructions

1. **Clone the Repository:** Clone this GitHub repository to your local machine.
2. **Install Dependencies:** Make sure you have Jupyter Notebook installed along with necessary libraries such as pandas, numpy, scikit-learn, and matplotlib.
3. **Open the Notebook:** Launch Jupyter Notebook and navigate to the cloned repository directory. Open the notebook file `arctic_penguins.ipynb`.
4. **Execute Cells:** Execute each cell in the notebook sequentially to perform data preprocessing, PCA analysis, determining the optimal number of clusters, performing K-means clustering, and visualizing the results.

## Conclusion

By following the steps outlined in this notebook, you can identify groups in the penguin dataset using K-means clustering. This approach helps in gaining insights into the characteristics of different penguin groups, even in the absence of species labels.

Happy clustering! 🐧🔍
