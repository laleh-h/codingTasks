# Predicting Insurance Costs Using Age: A Linear Regression Approach

## Description
This project explores the impact of age on insurance costs through the application of simple linear regression. By analyzing a dataset containing age and corresponding insurance costs, the model aims to predict insurance expenses based solely on age. The results highlight how age influences insurance premiums, providing valuable insights for both consumers and insurance companies. The project includes data preprocessing, model training, evaluation, and visualization of the relationship between age and insurance costs.

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
The dataset used in the insurance cost analysis is `insurance.csv` which contains information about individuals' demographics, lifestyle, and corresponding insurance charges. The dataset consists of 1,338 entries and 7 columns. The columns include:

- `age`: The age of the individual.
- `sex`: The gender of the individual (male/female).
- `bmi`: Body mass index, a measure of body fat based on height and weight.
- `children`: The number of children/dependents covered by the insurance.
- `smoker`: Whether the individual is a smoker (yes/no).
- `region`: The residential region of the individual in the US (northeast, northwest, southeast, southwest).
- `charges`: The medical insurance charges billed by the insurance company.

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
Open and run the `predict_insurance.ipynb` notebook. Follow the prompts and enter an age when requested. The model will then return the predicted insurance cost based on the age provided.