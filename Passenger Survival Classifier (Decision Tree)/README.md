# Titanic's Passengers Survival Prediction: A Decision Tree Classifier Approach  

## Description
This project utilizes a Decision Tree Classifier to predict passenger survival on the Titanic dataset. The sinking of the Titanic is one of the most infamous shipwrecks in history, and the dataset contains demographics and passenger information from 891 of the 2,224 passengers and crew on board. The goal of this project is to build a model that predicts whether a passenger survived or not based on attributes such as age, sex, ticket class, and more.

## Required Libraries
- `pandas`
- `numpy`
- `matplotlib.pyplot`
- `seaborn`
- `scipy.stats`
- `sklearn.preprocessing`
- `sklearn.model_selection`
- `sklearn.tree`
- `sklearn.metrics`

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
cd codingTasks/Passenger\ Survival\ Classifier\ \(Decision\ Tree\)/
```

- Run the Jupyter Notebook:

Launch Jupyter Notebook and open the `decision_tree_titanic.ipynb` file. Execute each cell to see the data preprocessing steps, model training, evaluation metrics, and visualizations.

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

### 5. Model Training
The decision tree classifier was trained on the training set, exploring various values of max_depth ranging from 2 to 10. This hyperparameter controls the maximum depth of the tree, influencing the model's complexity and ability to generalize to unseen data.

### 6. Model Evaluation
Evaluation of the decision tree classifier involved assessing its performance metrics, including:

- Confusion Matrix: Providing a detailed breakdown of true positive, false positive, true negative, and false negative predictions.
- Accuracy Score: Calculated to gauge the overall correctness of the classifier's predictions on the test set.

### 7. Visualization of Results
Visual representation of the decision tree was generated using plot_tree from `sklearn.tree`. This visualization offered insights into the hierarchical structure of the decision-making process employed by the classifier, highlighting key splits and decision nodes.