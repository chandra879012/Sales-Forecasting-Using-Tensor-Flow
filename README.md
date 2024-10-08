# Sales Forecasting Model

This repository contains a deep learning model for forecasting total sales based on various features, such as product type, city, operating profit, and units sold. The model is built using TensorFlow and Keras, with data preprocessing done using Scikit-learn.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Evaluation](#evaluation)
- [Saving and Loading the Model](#saving-and-loading-the-model)
- [Contributing](#contributing)

## Overview

This project aims to build a regression model that predicts future sales based on historical data. The model is trained using a dataset that includes various features such as product type, city, operating profit, and units sold.

## Dataset

The dataset used in this project contains the following features:
- **Product**: The type of product sold.
- **City**: The city where the product was sold.
- **Operating Profit**: The operating profit associated with the sale.
- **Units Sold**: The number of units sold.
- **Total Sales**: The target variable representing the total sales value.

The dataset undergoes preprocessing steps, including standard scaling for numerical features and one-hot encoding for categorical features.

## Model Architecture

The model is a deep learning neural network built with TensorFlow and Keras. It consists of:
- An input layer that takes in the preprocessed features.
- Two hidden layers with ReLU activation functions.
- An output layer that predicts the total sales.

## Installation

To run this project, you'll need Python 3.x and the following Python libraries:

- TensorFlow
- Keras
- Scikit-learn
- Pandas
- Matplotlib

You can install the required packages using pip:

```bash
pip install tensorflow scikit-learn pandas matplotlib
```

## Usage

1. **Training the Model**: 
   The model is trained using the provided dataset. You can run the training process by executing the provided notebook.

2. **Saving the Model**:
   After training, the model can be saved using the following code:
   ```python
   model.save('sales_forecasting_model.h5')
   ```

3. **Loading the Model**:
   To use the model later for prediction or further training:
   ```python
   from tensorflow.keras.models import load_model
   model = load_model('sales_forecasting_model.h5')
   ```

## Evaluation

The model is evaluated using Mean Absolute Error (MAE) on the test dataset. A scatter plot is also provided to visualize the model’s predictions against the actual sales values.

## Saving and Loading the Model

### Saving the Model
```python
model.save('sales_forecasting_model.h5')
```

### Loading the Model
```python
from tensorflow.keras.models import load_model
loaded_model = load_model('sales_forecasting_model.h5')
```

## Contributing

If you'd like to contribute to this project, please fork the repository and use a feature branch. Pull requests are welcome.

---


