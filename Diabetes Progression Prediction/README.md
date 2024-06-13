# Predicting Diabetes Progression: A Multiple Linear Regression Approach

## Description
This project develops a multiple linear regression model to predict the one-year progression of diabetes (PROGRESSION) using various demographic and health-related features. The features include age, sex, body mass index (BMI), average blood pressure (BP), and six blood serum measurements (S1-S6). By leveraging these predictors, the model aims to provide accurate predictions of diabetes progression, offering valuable insights for healthcare providers and patients.

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
- `joblib`

## Dataset

The dataset used in the diabetes progression analysis contains information about individuals' demographics, health metrics, and diabetes progression measurements. The dataset includes the following columns:

- `AGE`: The age of the individual.
- `SEX`: The gender of the individual (1 for male, 2 for female).
- `BMI`: Body mass index, a measure of body fat based on height and weight.
- `BP`: Average blood pressure.
- `S1-S6`: Six blood serum measurements.
- `PROGRESSION`: The target variable indicating the one-year progression of diabetes. It refers to the change or advancement in the severity or stage of diabetes over a one-year period. It is a measure of how much the condition of diabetes has worsened or improved for an individual within that timeframe.

## Key Steps and Importance

### 1. Data Exploration
Utilizes visual tools such as histograms, scatter plots, and box plots to understand the distribution and relationships within the dataset. Descriptive statistics provide measures like mean, median, and standard deviation. Data exploration helps uncover underlying patterns, detect anomalies, and understand the data's structure. It lays the groundwork for effective modeling by ensuring a deep understanding of the dataset.

### 2. Data Engineering
Applies transformations like normalization or standardization to numerical features to bring them onto a similar scale. Feature engineering, including scaling, improves model performance by ensuring that features contribute equally to the model, preventing dominance by features with larger magnitudes.

### 3. Correlation Matrix
Constructs a correlation matrix to identify the strength and direction of relationships between features and the target variable. Understanding correlations aids in feature selection, allowing the focus on features with the strongest predictive power and reducing the risk of multicollinearity.

### 4. Train-Test Split
Divides the dataset into training and testing subsets, in an 80/20 ratio. Splitting the data ensures that the model is trained on one subset and validated on another, which helps in assessing the model's performance on unseen data and prevents overfitting.

### 5. Model Training with Grid Search
Uses `GridSearchCV` to automate the process of tuning hyperparameters, testing various parameter combinations to find the best-performing model. Hyperparameter tuning is crucial for optimizing model performance, ensuring that the chosen model configuration yields the best results.

### 6. Model Evaluation
Calculates key evaluation metrics like mean-squared error (MSE) and r-squared (R²) to quantify model accuracy. These metrics provide insight into the model’s performance, with MSE measuring prediction error and R² indicating the proportion of variance explained by the model.

### 7. Visualization of Results
Visualizes the relationship between actual data points and the predictions made by the regression model. This plot helps in assessing the model’s fit and understanding how well the linear regression captures the underlying trend in the data.

### 8. Error Plotting
Creates error plot (residual plot), to visualize the discrepancies between predicted and actual values. Error plotting is essential for diagnosing issues like heteroscedasticity and identifying patterns in prediction errors, which can guide further model refinement.

### 9. Model Persistence
Persists the trained model using `joblib`, enabling future predictions without retraining.  Model persistence is critical for deploying the model in real-world applications, allowing for efficient and consistent predictions on new data.

## Run the model
Open and run the `predict_diabetes.ipynb` notebook. Follow the prompts and enter an age when requested. The model will then return the predicted insurance cost based on the age provided.

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
cd codingTasks/Diabetes\ Progression\ Prediction/
```

- Run the Jupyter Notebook:

Launch Jupyter Notebook and open the `diabetes_regression.ipynb` file. Execute each cell to see the data preprocessing steps, model training, evaluation metrics, and visualizations.