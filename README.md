# Delivery Time Prediction

A Python machine learning project that predicts food delivery time using delivery-related information such as distance, preparation time, traffic level, and rain.

## Features

- Load and split the delivery dataset
- Calculate delivery-related features
- Train a Linear Regression model
- Evaluate the model using Mean Absolute Error (MAE)
- Save and load the trained model using Joblib
- Validate delivery orders
- Predict delivery time for a new order
- Run training and prediction from the command line

## Project Structure

```text
delivery-time-prediction/
│
├── delivery/
│   ├── __init__.py
│   ├── data.py
│   ├── features.py
│   ├── model.py
│   └── validate.py
│
├── train.py
├── predict.py
├── model.joblib
└── README.md
Input Features
distance_km — Delivery distance in kilometres
prep_time_min — Food preparation time in minutes
traffic_level — Traffic level from 1 to 3
rain — Rain condition (0 or 1)
Target
delivery_min — Delivery time in minutes
Machine Learning Model

The project uses Linear Regression to predict delivery time.

The dataset is divided into training and testing sets using an 80:20 split.

The model is evaluated using Mean Absolute Error (MAE).

Validation

An order is considered valid if:

Distance is greater than 0
Preparation time is greater than or equal to 0
Traffic level is 1, 2, or 3
Rain is 0 or 1
Installation

Install the required Python libraries:

pip install numpy pandas scikit-learn joblib
Usage
Train the Model
python train.py
Make a Prediction
python predict.py

The prediction script uses a sample delivery order and prints the predicted delivery time.

Technologies Used
Python
NumPy
Pandas
Scikit-learn
Joblib
Jupyter Notebook
