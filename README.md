# Data Analysis and Classification with KMeans++

## 1. Exploratory Data Analysis Report

The first step in performing an Exploratory Data Analysis (EDA) is preparing the dataset. This dataset is one of the earliest used in classification literature and is widely applied in statistics and machine learning. It contains three classes with 50 instances each, where each class represents a specific type of iris plant.

To facilitate working with the data, a header row was added to the dataset to indicate what each column represents.


### Dataset Profiling Report

After profiling the dataset, we generated a detailed report that includes:

- **Dataset Statistics:**
  A series of statistical insights is obtained, providing a general overview of the dataset's structure. This allows us to identify potential challenges that may arise in future analyses.

  ![image](https://github.com/user-attachments/assets/a7c74292-bb2b-47e0-a8dd-78b53d85c946)

- **Alerts and Possible Errors:**
  The profiling library highlights data patterns that might cause issues when used in a machine learning model.

  <img width="904" alt="Captura de pantalla 2024-09-10 a la(s) 11 16 12 a m" src="https://github.com/user-attachments/assets/14e1b428-04b5-4d46-8a4a-b9c43c64ebc5">

- **Variable Analysis:**
  Each column is individually analyzed to display its maximum, minimum, and potential outliers that may need to be modified or removed.

  <img width="932" alt="Captura de pantalla 2024-09-10 a la(s) 11 31 41 a m" src="https://github.com/user-attachments/assets/aeafc2b9-d6c9-4291-876f-bda873c08296">

- **Interactions:**
  Scatter plots of each variable are generated, showing how they interact with each other across the dataset.

- **Correlations:**
  A correlation matrix is displayed, showing the correlation coefficients between variables. This matrix helps summarize large datasets and reveals patterns between pairs of variables.

  <img width="845" alt="Captura de pantalla 2024-09-10 a la(s) 12 16 57 p m" src="https://github.com/user-attachments/assets/b475423c-c219-4a84-b359-33efe0dc7039">


## 2. Classification with KMeans++

We used the KMeans++ algorithm from the `Sklearn` library to classify the dataset. KMeans++ is a clustering method aimed at partitioning a set of `n` observations into `k` clusters, where each observation belongs to the cluster with the nearest mean. In this case, the algorithm was set to group the data into 3 clusters based on 4 features, excluding the "species" label, which was discarded.

### Principal Component Analysis (PCA)

PCA was used to reduce the dimensionality of the original data while preserving as much variability as possible. In this case, the data was reduced to 2 components (X, Y) for visualization purposes.

  ![image](https://github.com/user-attachments/assets/2703f776-f5d7-4425-9ff1-f14d5730da8e)

### Cluster Visualization

The resulting clusters are visualized, showing how each data point was classified. This visualization helps to observe the relationships between the nearest data points and the resulting clusters.

  ![image](https://github.com/user-attachments/assets/3f76f2d5-838e-4ed6-9e90-66a01c0d593e)




