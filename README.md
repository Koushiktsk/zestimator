House Price Prediction Project

Overview

This project is a machine learning web application that predicts house prices based on user inputs such as location, total square feet, number of bedrooms (BHK), and number of bathrooms. The application leverages a Random Forest Regressor model and is deployed using Flask for the backend. Users can interact with the application via a web interface to get estimated prices for houses in a specific city (e.g., Bengaluru).

Features

Machine Learning: Predict house prices using a trained model.

User Input: Input features such as location, total square feet, BHK, and bathrooms.

Interactive Web App: Developed with Flask to provide a simple and intuitive interface.

Preprocessing: Efficiently processes and uses real-world housing data.

Technology Stack

Programming Language: Python

Libraries:

Flask: For backend and web server.

Pandas: For data preprocessing and manipulation.

Scikit-learn: For building and training the machine learning model.

NumPy: For numerical operations.

Matplotlib/Seaborn: For data visualization (during development).

Pickle: To save and load the trained model.

Frontend: HTML/CSS (via Flask templates)

Deployment Platform: Can be hosted locally or on platforms like Heroku.

Dataset

Source: The dataset used in this project contains real estate data such as house prices, location, square feet, number of bedrooms, and bathrooms.

Features:

Location

Total_sqft

BHK

Bath

Price (Target Variable)

The dataset was cleaned and preprocessed to remove outliers and handle missing data.

Installation and Setup

Prerequisites

Python 3.7 or higher

Libraries mentioned in the requirements.txt

Steps to Run the Application

Clone the repository:

git clone https://github.com/your-username/house-price-predictor.git
cd house-price-predictor

Install dependencies:

pip install -r requirements.txt

Run the Flask application:

python server.py

Open your browser and go to:

http://127.0.0.1:5000/

How It Works

Input:

The user provides inputs such as location, total square feet, BHK, and bathrooms via a form on the web app.

Model:

The input data is processed and passed to a pre-trained Random Forest Regressor model.

Prediction:

The model predicts the price based on the input features and displays the estimated price on the web interface.

Files and Directories

server.py: Main Flask application file.

util.py: Contains helper functions for preprocessing and prediction.

artifacts/: Directory containing saved models and other necessary files.

model.pkl: The trained Random Forest Regressor model.

columns.json: JSON file containing information about feature columns.

templates/: Contains HTML templates for the web interface.

app.html: Main web page for user input.

requirements.txt: List of required Python libraries.

static/: Directory for static files like CSS and images (if applicable).

Future Improvements

Add more features to improve model accuracy (e.g., amenities, age of the property).

Use advanced machine learning models like Gradient Boosting or XGBoost.

Add data visualization to show trends in house prices.

Deploy the application on a cloud platform like Heroku or AWS.

Optimize the model using hyperparameter tuning.

License

This project is licensed under the MIT License. You are free to use and modify it.

Acknowledgments

Data Source: Real estate datasets (Bengaluru housing data or similar).

Libraries: Scikit-learn, Flask, Pandas, NumPy.

