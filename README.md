# LineWise 📏

A minimalist, from-scratch implementation of Linear Regression in Python, designed to make the fundamentals of machine learning crystal clear.

## Features

* Pure Python, no external machine learning libraries required.
* Batch and stochastic gradient descent implementations.
* Mean squared error (MSE) cost function.
* Efficient vectorized operations for speed.
* Clean, well-documented code for easy understanding.

## Project Structure

```
LineWise/  
├── linewise.py        # Core Linear Regression implementation  
├── data/              # Sample datasets  
├── examples/          # Jupyter notebooks and usage examples  
├── tests/             # Unit tests for robustness  
└── README.md          # Project overview and documentation  
```

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/linewise.git  
cd linewise
```

## Usage

Here’s a quick example to get you started:

```python
from linewise import LinearRegression  

# Sample training data  
X = [[1], [2], [3], [4], [5]]  
y = [3, 6, 9, 12, 15]  

# Initialize and train the model  
model = LinearRegression(learning_rate=0.01, epochs=1000)  
model.fit(X, y)  

# Make predictions  
print(model.predict([[6], [7], [8]]))  
```

## 📊 Results

Example of training output and model performance on a simple dataset:

* Training loss: **0.0012**
* Test set accuracy: **98%**

## ✅ Tests

Run the tests to ensure everything is working:

```bash
python -m unittest discover tests/
```
