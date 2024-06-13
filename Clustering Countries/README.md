# Categorising Countries: A K-means Clustering Approach

## Description
This project utilizes K-means clustering, an unsupervised machine learning algorithm, to group countries based on various socio-economic and health factors. The goal is to classify countries into different clusters that reflect their development status. By analyzing these clusters, we can gain insights into the similarities and differences among countries regarding their development and identify patterns that can inform policy and decision-making.

## Required Libraries
- `pandas`
- `numpy`
- `matplotlib.pyplot`
- `seaborn`
- `scipy.stats`
- `sklearn.preprocessing`
- `sklearn.cluster`
- `sklearn.metrics`

## Dataset
The dataset used in the project consists of 167 enteries of various socio-economic and health indicators for multiple countries. The goal of this dataset is to provide a comprehensive view of the factors influencing the development status of each country. Below is a detailed description of the dataset and its features:

- `Country`: The name of the country.
- `Child Mortality`: Number of deaths per 1,000 children under the age of 5.
- `Exports`: Value of exports as a percentage of GDP.
- `Health`: Total expenditure on health as a percentage of GDP.
- `Imports`: Value of imports as a percentage of GDP.
- `Income`: Net income per person.
- `Inflation`: The annual inflation rate.
- `Life Expectancy`: The average number of years a person is expected to live.
- `Total Fertility`: The average number of children born to a woman over her lifetime.
- `GDPP`: Gross Domestic Product per capita.
- `Population`: The total population of the country.

## Key Steps and Importance

### 1. Data Exploration
Conducted an initial examination of the dataset to understand its structure, distribution, and key statistics. This included summarizing the data, checking for missing values, and identifying potential outliers.
### 2. Data Engineering
Applied winsorization to limit extreme values in the dataset, reducing the influence of outliers without completely removing them.
Standardized the data using techniques like z-score normalization or min-max scaling to ensure all features contribute equally to the clustering process.
### 3. Correlation Matrix
Created a correlation matrix to assess the relationships between different socio-economic and health factors. This helped identify highly correlated features, which can be useful for understanding the underlying structure of the data and for feature selection.
### 4. Feature Selection
Based on the correlation analysis and domain knowledge, selected the most relevant features that significantly contribute to determining a country's development status. This step ensured that the model focused on the most informative variables.
### 5. Selecting K (Number of Clusters)
Used the Elbow method to determine the optimal number of clusters. Plotted the within-cluster sum of squares (WCSS) against the number of clusters and looked for an 'elbow point' where the rate of decrease slows down.
Performed Silhouette analysis to validate the optimal number of clusters by measuring how similar an object is to its own cluster compared to other clusters.
### 6. Model Fitting
Applied the K-means clustering algorithm to the preprocessed dataset using the selected number of clusters. Iteratively assigned data points to clusters and updated the cluster centroids until convergence.
### 7. Adding Clusters to the Original Dataset
Added the cluster labels obtained from the K-means model to the original dataset. This step allowed for the examination of the clustering results in the context of the original data.
Analyzed the characteristics of each cluster by examining the distribution of features within each group and identifying common traits.
### 8. Visualization of Clusters
Created scatter plots to visualize the clusters in two-dimensional space, using different feature pairs (gdpp vs child_mort and gdpp vs inflation) to highlight the separation and cohesion of clusters.
### 9. Clusters Mapping
Assigned descriptive names to each cluster based on the socio-economic and health characteristics identified by the model. For example:
Cluster 0: 'Developing'
Cluster 1: 'Developed'
Cluster 2: 'Least Developed'

## Installation
To get started with the projects in this repository, follow these steps:

- Clone the repository:
```
git clone https://github.com/laleh-h/codingTasks.git
```

Install dependencies:
Ensure you have Python 3.x and pip installed. Install the required libraries using:

```
pip install -r requirements.txt
```

## Usage
- Navigate to the project directory:
```
cd codingTasks/Clustering\ Countries/
```

- Run the Jupyter Notebook:

Launch Jupyter Notebook and open the `countries_clustering.ipynb` file. Execute each cell to see the data preprocessing steps, model training, evaluation metrics, and visualizations.