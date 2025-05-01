# prj_car_price_predictions


# Car Price Prediction

This is an end-to-end machine learning project that predicts the price of used cars. It includes data storage using MySQL, model training using RandomForestRegressor, and deployment using a Streamlit web app.

## Project Overview

The goal of this project is to create a machine learning pipeline that can predict car prices based on various input features such as model, year, fuel type, mileage, engine size, transmission type, and owner count.

## Dataset Information

The dataset contains the following columns:

- Model
- Year
- Engine_Size
- Fuel_Type
- Transmission
- Mileage
- Owner_Count
- Price (Target Variable)

## Technologies Used

- Python
- MySQL
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Streamlit
- Joblib, Pickle
- GitHub

## Steps Followed

### 1. Data Storage
- The dataset was uploaded and stored in MySQL Workbench.
- Connected to MySQL using pymysql and loaded the data into a pandas DataFrame.

### 2. Exploratory Data Analysis (EDA)
- Checked for missing values and outliers.
- Used histograms, box plots, and correlation heatmaps for visual analysis.
- Cleaned and prepared the data for modeling.

### 3. Feature Engineering
- Applied one-hot encoding to categorical columns (Model, Fuel_Type, Transmission).

### 4. Model Building
- Used RandomForestRegressor for prediction.
- Trained the model using train_test_split.
- Evaluated the model using MAE, MSE, R2 Score and RMSE.
- Saved the model as `rfr_cars_price_pred_compressed.pkl`.
- Saved the feature columns as `columns.pkl`.

### 5. Streamlit App Development
- Built an interactive web app using Streamlit.
- App takes user input and displays the predicted car price.

## How to Run

1. Clone the repository:
```
git clone https://github.com/khizareen/car-price-predictor.git
cd car-price-predictor
```

2. Install dependencies:
```
pip install -r requirements.txt
```

3. Run the Streamlit app:
```
streamlit run app.py
```

## Repository Contents

- `app.py` - Streamlit web app
- `rfr_cars_price_pred_compressed.pkl` - Trained model file
- `columns.pkl` - Encoded feature columns
- `requirements.txt` - Python dependencies
- `cars_price.sql` - MySQL dump of dataset
- `README.md` - Project documentation

## Deployment

The app is deployed on Streamlit Cloud.  
**Live URL**: (https://prjcarpricepredictions-5cfucfygug34egrxzcey6v.streamlit.app/)

## Author

Your Name  
GitHub: [https://github.com/yourusername](https://github.com/yourusername)
