# PCA and Clustering Analysis with Delta Airlines Fleet

This project thoroughly analyzes the aircraft in Delta Airlines' fleet to identify similarities and differences among the various models. The analysis involves data loading, visualization, Principal Component Analysis (PCA), and clustering.

### Highlights:
1. Data Inspection: Load and inspect aircraft data from Delta Airlines.
2. Correlation Analysis: Scatterplots are used to visualize pairwise correlations among aircraft characteristics such as cruising speed, range, and wingspan.
3. PCA: Standardize data and reduce dimensionality to capture the most significant features with minimal information loss.
4. Clustering: Implement k-means clustering to group similar aircraft and visualize these clusters using elbow curves and scatter plots of principal components.

### Key Components:
- PCA Execution: Calculate the variance explained by each principal component and visualize the cumulative variance to determine the optimal number of components.
- Cluster Analysis: Determine the best number of clusters using the elbow method and perform k-means clustering to categorize the aircraft into distinct groups.

### PCA (Principal Component Analysis)
**Principal Component Analysis (PCA)** is a statistical technique used in data science for dimensionality reduction while preserving as much variability in the data as possible. 
It transforms the data into a new coordinate system with "principal components), ordered by the amount of the variance they capture from the data (hence, the first principal component captures the most variance).

### Cumulative Variance Curve
The **cumulative variance curve** in PCA is to determine how many principal components are needed to adequately represent the data. This curve shows the cumulative sum of the variance explained by each successive principal component.
By observing where the curve starts to plateau (or when it reaches certain percentage of the total variance), we can select the smallest number of components that capture the majority of the variability of the data.

This approach allows for a significant reduction in the dataset's dimensionality with minimal loss of information, which is crucial for further data analysis.

In our case (graph below), the first principal component alone accounts for 60% of the variance, by the time we include the 3rd principal component, over 90% of the variance is explained

![pca](https://github.com/YenChenHsu/PCA-and-Clustering-Analysis/assets/57134574/ed4c3ba8-600f-4ec2-b7d6-c7379f66913b)


