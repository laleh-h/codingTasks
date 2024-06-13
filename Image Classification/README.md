# Handwritten Digit Classification using MNIST Dataset with RandomForest Classifier

## Description
This project develops a machine learning model capable of accurately classifying handwritten digits using the MNIST dataset. This involves preprocessing the images to enhance their quality, applying contrast stretching, and flattening the images for analysis. The project aims to split the data into training and testing sets, ensuring the model is trained effectively and evaluated on unseen data. By implementing these steps, the project seeks to achieve high classification accuracy and demonstrate the practical application of image preprocessing and machine learning techniques in digit recognition tasks.

## Required Libraries
- `numpy`
- `sklearn.datasets`
- `sklearn.skimage`
- `sklearn.preprocessing`
- `sklearn.model_selection`
- `sklearn.metrics`
- `sklearn.ensemble`

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
cd codingTasks/Image\ Classification/
```

- Run the Jupyter Notebook:

Launch Jupyter Notebook and open the `digital_image_classifier.ipynb` file. Execute each cell to see the data preprocessing steps, model training, evaluation metrics, and visualizations.

## Dataset
The MNIST (Modified National Institute of Standards and Technology) dataset is a widely used benchmark in the field of machine learning and computer vision. It consists of a large collection of 1,797 8x8 pixels handwritten digits that is commonly used for training various image processing systems. Below is a detailed description of the MNIST dataset available in the sklearn.datasets module:

- Images: Each image is a grayscale image of size 8x8 pixels, representing a single handwritten digit.
- Labels: Corresponding to each image, there is a label that indicates the digit (0-9) shown in the image.

## Key Steps and Importance

### 1. Data Exploration


### 2. Train-Test Split

### 3. Image Processing
Contrast stretching, also known as normalization, is a technique used to enhance the contrast of an image by stretching the range of intensity values it contains. It redistributes the pixel values to utilize the entire possible range, typically from 0 to 255 for 8-bit images. Contrast stretching improves the visibility of features in the image, making it easier for both humans and algorithms to detect important details.

Contrast stretching Process:

- Identify Percentiles: Calculate the lower and upper percentiles (e.g., 2nd and 98th percentiles) of the pixel intensities.
- Rescale Intensities: Stretch the pixel values such that the lower percentile maps to 0 and the upper percentile maps to 255, enhancing the overall contrast of the image.

Flattening is the process of converting a multi-dimensional array (e.g., a 2D image) into a one-dimensional array (vector). Each pixel’s intensity value is retained, but the spatial structure of the image is removed. Many machine learning models require a fixed-size 1D input. Flattening ensures compatibility with these models.

Flattening Process:

- Reshape Array: Convert the 2D array of pixel values into a 1D array.
- Preserve Data: Ensure that all pixel intensity values are included in the new array.

### 5. Model Training with Grid Search
Random Forest generally provides high accuracy and handles overfitting better than individual decision trees. The Random Forest classifier was trained and tested on the preprocessed MNIST dataset. The classifier was evaluated with n_estimators values of 50, 100, and 150 to find the optimal number of trees for the best performance.

### 6. Model Evaluation
A confusion matrix is  used to evaluate the performance of the model. It summarizes the counts of true positives, true negatives, false positives, and false negatives, providing a detailed insight into the model's performance.