# Titanic's Passengers Survival Prediction: A Random Forest Classifier Approach  

## Description
This project aims to predict the survival of passengers on the Titanic using a Random Forest Classifier. By leveraging the well-known Titanic dataset, this project demonstrates the application of machine learning techniques to classify passengers based on various features such as age, sex, class, and more.

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
cd codingTasks/Passenger\ Survival\ Classifier\ \(Random\ Forest\)/
```

- Run the Jupyter Notebook:

Launch Jupyter Notebook and open the `random_forest_titanic.ipynb` file. Execute each cell to see the data preprocessing steps, model training, evaluation metrics, and visualizations.

## Dataset
- `Survived`: Survival (0 = No, 1 = Yes)
- `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Name`: Passenger's name
- `Sex`: Passenger's sex
- `Age`: Passenger's age in years
- `SibSp`: Number of siblings/spouses aboard the Titanic
- `Parch`: Number of parents/children aboard the Titanic
- `Ticket`: Ticket number
- `Fare`: Passenger fare
- `Cabin`: Cabin number
- `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Key Steps and Importance

### 1. Data Exploration
Initial exploration of the Titanic dataset was conducted to understand its structure and contents. This included examining the shape of the dataset and reviewing sample records to gain insights into the available features.

### 2. Data Preprocessing
Prior to modeling, thorough data preprocessing steps were implemented:

- Handling Missing Values: Missing data points were identified and addressed using appropriate strategies such as imputation.
- Encoding Categorical Variables: Categorical features like sex and embarked port were encoded to numerical values suitable for machine learning algorithms.
- Feature Scaling: Continuous features were standardized to ensure all variables were on a similar scale, preventing any particular feature from dominating the model training process.

### 4. Data Splitting
To effectively train, validate, and test the model's performance, the dataset was split into three distinct sets:

- Training: Used to train the decision tree classifier.
- Validation (Development): Employed for hyperparameter tuning, allowing adjustment of parameters such as max_depth.
- Test: Reserved to provide an unbiased evaluation of the model's performance after training and validation.

### 5. Model Training with Grid Search
   - Implementation of Random Forest, AdaBoost, and Bagging classifiers.
   - Evaluation of each model to determine the optimal configuration.

