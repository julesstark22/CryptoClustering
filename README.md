# CryptoClustering

The code generates various plots and outputs the cluster labels for each cryptocurrency.

Code Explanation
Data Loading and Exploration

The market data is loaded from a CSV file using pandas.
Summary statistics and sample data are displayed to get an overview of the dataset.
A line plot is created to visualize the data.
Data Preparation

The data is normalized using the StandardScaler module from scikit-learn.
A DataFrame is created with the scaled data.
Crypto names are copied from the original data and set as the index.
Finding the Best Value for k Using the Original Data

Inertia values are computed for different values of k (number of clusters).
An elbow curve is plotted to identify the optimal value for k.
Cluster Cryptocurrencies with K-means Using the Original Data

K-Means clustering is performed with the best value of k.
Cluster labels are predicted for the data.
The cluster labels are added as a new column to the DataFrame.
A scatter plot is created to visualize the clusters.
Optimizing Clusters with Principal Component Analysis (PCA)

PCA is applied to reduce the dimensionality of the data.
The explained variance ratio is computed to determine the information attributed to each principal component.
The data is transformed using PCA, and a new DataFrame is created.
The PCA-transformed data is used for further analysis.
Finding the Best Value for k Using the PCA Data

Inertia values are computed for different values of k using PCA-transformed data.
An elbow curve is plotted to identify the optimal value for k.
Cluster Cryptocurrencies with K-means Using the PCA Data

K-Means clustering is performed with the best value of k obtained from the PCA analysis.
Cluster labels are predicted for the PCA-transformed data.
The cluster labels are added as a new column to the PCA DataFrame.
A scatter plot is created to visualize the clusters.
Visualizing and Comparing the Results

Elbow curves are plotted to compare the clustering results using the original data and PCA-transformed data.
Scatter plots are created to visualize and compare the clusters obtained from the original data and PCA data.
