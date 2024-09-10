# Data Analysis and Classification with KMeans++

## 1. Exploratory Data Analysis Report

The first step in performing an Exploratory Data Analysis (EDA) is preparing the dataset. This dataset is one of the earliest used in classification literature and is widely applied in statistics and machine learning. It contains three classes with 50 instances each, where each class represents a specific type of iris plant.

To facilitate working with the data, a header row was added to the dataset to indicate what each column represents.

### Dataset Profiling Report

After profiling the dataset, we generated a detailed report that includes:

- **Dataset Statistics:**
  A series of statistical insights is obtained, providing a general overview of the dataset's structure. This allows us to identify potential challenges that may arise in future analyses.

- **Alerts and Possible Errors:**
  The profiling library highlights data patterns that might cause issues when used in a machine learning model.

- **Variable Analysis:**
  Each column is individually analyzed to display its maximum, minimum, and potential outliers that may need to be modified or removed.

- **Interactions:**
  Scatter plots of each variable are generated, showing how they interact with each other across the dataset.

- **Correlations:**
  A correlation matrix is displayed, showing the correlation coefficients between variables. This matrix helps summarize large datasets and reveals patterns between pairs of variables.

## 2. Classification with KMeans++

We used the KMeans++ algorithm from the `Sklearn` library to classify the dataset. KMeans++ is a clustering method aimed at partitioning a set of `n` observations into `k` clusters, where each observation belongs to the cluster with the nearest mean. In this case, the algorithm was set to group the data into 3 clusters based on 4 features, excluding the "species" label, which was discarded.

### Principal Component Analysis (PCA)

PCA was used to reduce the dimensionality of the original data while preserving as much variability as possible. In this case, the data was reduced to 2 components (X, Y) for visualization purposes.

### Cluster Visualization

The resulting clusters are visualized, showing how each data point was classified. This visualization helps to observe the relationships between the nearest data points and the resulting clusters.

