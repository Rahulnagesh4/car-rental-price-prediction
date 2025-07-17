# car-rental-price-prediction
This project focuses on predicting car rental prices using advanced machine learning techniques. It leverages vehicle features, customer reviews, and location data to build accurate models that support pricing strategy optimization in the car rental industry.

Objectives
Predict car rental prices based on vehicle and location data.

Compare the performance of Multiple Regression, Random Forest, and XGBoost models.

Identify key features that impact rental prices.

Enable data-driven decision-making for dynamic pricing strategies.


Files
car_rental_price_prediction.py – Main Python script for data preprocessing, model training, and evaluation.

CarRentalDataV1.csv – Dataset containing vehicle and rental information.


The dataset includes:

Vehicle Details: make, model, year, type, fuel type.

Customer Info: rating, number of trips, review count.

Location: city, state, latitude, longitude.

Target: daily rental price.



 Techniques Used
Data Preprocessing: Handling missing values, one-hot encoding, scaling.

Feature Engineering: Geographic encoding, transformation of categorical variables.

Model Tuning: RandomizedSearchCV for hyperparameter optimization.

Evaluation Metrics: R² score and RMSE.


Future Enhancements
Integrate real-time pricing data from APIs.

Deploy model using a web interface or REST API.

Incorporate external factors (e.g., weather, local events) for more accurate pricing.
