# Logic Gates: The Power of Neural Networks

## Description
This project demonstrates the capabilities of neural networks by modeling logic gates, which are the fundamental building blocks of digital computing. The notebook guides you through the process of using neurons to represent these gates and explains how to express neural networks through matrix computations.

## Required Libraries
- `numpy`
- `matplotlib.pyplot`

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
cd codingTasks/Logic\ Gates\ with\ ANN/
```

- Run the Jupyter Notebook:

Launch Jupyter Notebook and open the `neural_network_task.ipynb` file. Execute each cell to see the data preprocessing steps, model training, evaluation metrics, and visualizations.

## Dataset
This project does not utilize any external data sources. Instead, it generates and manipulates data manually within the project. This approach allows for customized data creation tailored specifically to the project's requirements and objectives.

## Key Components

1. **Introduction to Neural Networks**:
   - An overview of how neurons can be used to model logic gates.
   - Discussion on the representation of neural networks in terms of matrix operations.

2. **Neurons as Logic Gates**:
   - Explanation of how a neuron functions by applying an activation function (such as the sigmoid function) to a combination of inputs, weights, and a bias.
   - Implementation of a basic neuron class in Python.

3. **Sigmoid Function**:
   - A reminder of the sigmoid function and its mathematical representation:
     
     $$
     \sigma = \frac{1}{1 + e^{-x}}
     $$

## Project Structure

1. **Data Generation and Manipulation**:
   - This project does not rely on external data sources. Instead, data is generated and manipulated manually within the project to suit the requirements of demonstrating neural network concepts.

2. **Code Implementation**:
   - Python code snippets are provided to implement neurons and simulate their behavior as logic gates.
   - Visualization of results using `matplotlib`.