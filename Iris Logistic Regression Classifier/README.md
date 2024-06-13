# Predicting Iris Classification: A Logistic Regression Approach

## Description
The goal of this project is to develop a classifier using logistic regression to predict whether an iris flower belongs to the Iris-setosa class or not. The Iris dataset is a classic dataset in machine learning and contains measurements of iris flowers, including sepal and petal dimensions. By training a logistic regression model on this dataset, the project aims to accurately classify iris flowers based on their features. This serves as a fundamental exercise in binary classification, showcasing how logistic regression can be applied to distinguish between different classes within a dataset. The outcome provides insights into the feasibility and accuracy of using logistic regression for similar classification tasks in broader applications of machine learning.

## Required Libraries
- `pandas`
- `numpy`
- `matplotlib.pyplot`
- `seaborn`
- `scipy.stats`
- `sklearn.preprocessing`
- `sklearn.model_selection`
- `sklearn.linear_model`
- `sklearn.metrics`

## Dataset

The Iris dataset is a well-known and widely used dataset in the field of machine learning and statistics. It consists of 150 samples of iris flowers, each belonging to one of three species: `Iris-setosa`, `Iris-versicolor`, and `Iris-virginica`. The dataset includes the following features for each sample:

- `Id`
- `Sepal Length (cm)`
- `Sepal Width (cm)`
- `Petal Length (cm)`
- `Petal Width (cm)`
- `Species`

Each sample is labeled with its corresponding species, making the dataset ideal for supervised learning tasks, particularly classification. 

## Key Steps and Importance

### 1. Data Exploration
Utilizes visual tools such as histograms, scatter plots, and box plots to understand the distribution and relationships within the dataset. Descriptive statistics provide measures like mean, median, and standard deviation. Data exploration helps uncover underlying patterns, detect anomalies, and understand the data's structure. It lays the groundwork for effective modeling by ensuring a deep understanding of the dataset.

### 2. Data Engineering
Applies transformations like normalization or standardization to numerical features to bring them onto a similar scale. Feature engineering, including scaling, improves model performance by ensuring that features contribute equally to the model, preventing dominance by features with larger magnitudes.

### 3. Correlation Matrix
Constructs a correlation matrix to identify the strength and direction of relationships between features and the target variable `Species`. Understanding correlations aids in feature selection, allowing the focus on features with the strongest predictive power and reducing the risk of multicollinearity.

### 4. Train-Test Split
Divides the dataset into training and testing subsets, in an 80/20 ratio. Splitting the data ensures that the model is trained on one subset and validated on another, which helps in assessing the model's performance on unseen data and prevents overfitting.

### 5. Model Training with Grid Search
Uses `GridSearchCV` to automate the process of tuning hyperparameters, testing various parameter combinations to find the best-performing model. Hyperparameter tuning is crucial for optimizing model performance, ensuring that the chosen model configuration yields the best results.

### 6. Model Evaluation
Evaluation of the logistic regression classifier involved assessing its performance metrics, including:

- Confusion Matrix: Providing a detailed breakdown of true positive, false positive, true negative, and false negative predictions.
- Accuracy Score: Calculated to gauge the overall correctness of the classifier's predictions on the test set.

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
cd codingTasks/Iris\ Logistic\ Regression\ Classifier/
```

- Run the Jupyter Notebook:

Launch Jupyter Notebook and open the `iris_logistic_regression.ipynb` file. Execute each cell to see the data preprocessing steps, model training, evaluation metrics, and visualizations.