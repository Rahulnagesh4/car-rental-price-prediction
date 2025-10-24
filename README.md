# 🚗 Car Rental Price Prediction and Optimization

This project develops a **machine learning–based predictive model** to forecast car rental prices by analyzing various vehicle, location, and customer factors.  
It aims to optimize pricing strategies in the competitive car rental industry through **data-driven insights and predictive analytics**.

The study compares multiple models — **Multiple Regression**, **Random Forest**, and **XGBoost** — and identifies **XGBoost with hyperparameter tuning** as the most accurate algorithm for predicting rental costs.

---

## 📌 Key Objectives

- Build a predictive system for car rental pricing using machine learning.  
- Identify key factors influencing rental prices such as:
  - Vehicle specifications (make, model, year, fuel type)
  - Customer ratings and review counts
  - Location and geographic factors
- Compare multiple machine learning models for accuracy.
- Optimize the top-performing model through **Randomized Search CV** hyperparameter tuning.
- Support **data-driven pricing strategies** for the car rental industry.

---

## 🗂️ Dataset

The dataset was sourced from [Kaggle – Cornell Car Rental Dataset](https://www.kaggle.com/datasets/kushleshkumar/cornell-car-rental-dataset).  
It includes detailed records of vehicles and rental prices across multiple U.S. locations.

### Key Features

| Field | Description |
|--------|-------------|
| `vehicle.make` | Car manufacturer (e.g., Toyota, BMW, Ford) |
| `vehicle.model` | Model name |
| `vehicle.type` | Vehicle category (car, SUV, van, etc.) |
| `vehicle.year` | Manufacturing year |
| `fuelType` | Type of fuel (Gasoline, Hybrid, Electric, Diesel) |
| `rating` | Customer rating of the vehicle |
| `reviewCount` | Number of reviews |
| `renterTripsTaken` | Number of trips taken |
| `location.city`, `location.state` | Rental location details |
| `rate.daily` | Daily rental price (target variable) |

---

## 🛠️ Technologies Used

- **Python**
- **Scikit-Learn**
- **XGBoost**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

---

## 📊 Methodology

### 1. Data Preprocessing
- Handled missing values using **mean/mode imputation**.
- Encoded categorical variables via **One-Hot Encoding**.
- Scaled numeric features using **MinMaxScaler** and **StandardScaler**.

### 2. Feature Engineering
- Created location-based and fuel-type interaction features.
- Removed duplicates and inconsistent records.
- Performed **correlation analysis** to reduce multicollinearity.

### 3. Model Development
- Implemented and compared:
  - Multiple Linear Regression  
  - Random Forest Regressor  
  - XGBoost Regressor  
- Used **RandomizedSearchCV** for hyperparameter tuning.

### 4. Model Evaluation Metrics
- **R² (Coefficient of Determination)**
- **RMSE (Root Mean Squared Error)**

---

## 🧮 Results Summary

| Model | R² Score | RMSE |
|--------|-----------|------|
| Multiple Regression | 0.577 | 62.45 |
| Random Forest | 0.666 | 55.51 |
| XGBoost | 0.693 | 53.18 |
| **XGBoost (Tuned)** | **0.715** | **51.23** |

➡️ **XGBoost with hyperparameter tuning** achieved the best performance, explaining **71.5% of variance** in rental prices with the lowest prediction error.

---

## 📈 Data Insights

- **Tesla** and **Toyota** dominate the rental market, followed by **BMW** and **Ford**.  
- **Gasoline vehicles** make up **83.5%** of rentals, but **Electric** and **Hybrid** vehicles are steadily growing.  
- **California, Florida, and Texas** lead in rental availability.  
- Vehicle attributes, geographic location, and customer ratings significantly influence pricing.

---

## 🧠 Key Findings

- **XGBoost** outperforms traditional regression models due to its ability to handle **non-linear relationships** and **feature interactions**.  
- **Feature engineering** and **hyperparameter tuning** significantly improve model accuracy.  
- Machine learning enables **dynamic pricing optimization**, providing car rental companies with actionable insights to balance demand and profitability.

---

## 🔮 Future Work

- Integrate **real-time data** for dynamic price adjustments.  
- Include **external factors** such as weather, events, or competitor prices.  
- Develop a **Streamlit or Flask dashboard** for live prediction and visualization.  
- Add **sentiment analysis** on customer reviews to refine predictions.

---

## 📚 References

- Nagesh, R. (2024). *Predictive Analysis for Rental Price Optimisation in the Car Rental Industry*. University of Essex, School of Mathematics, Statistics and Actuarial Science.  
- Chen, T., & Guestrin, C. (2016). *XGBoost: A Scalable Tree Boosting System.* ACM SIGKDD.  
- Breiman, L. (2001). *Random Forests.* Machine Learning, 45(1):5–32.  
- Montgomery, D. C., Peck, E. A., & Vining, G. G. (2012). *Introduction to Linear Regression Analysis.* John Wiley & Sons.  
- Kumar, K. (2021). *Cornell Car Rental Dataset.* Kaggle.  

---

## 🧠 Skills Demonstrated

Machine Learning • Regression Modeling • Feature Engineering • XGBoost • Random Forest • Hyperparameter Tuning •  
Data Preprocessing • Data Visualization • Predictive Analytics • Dynamic Pricing • Statistical Modeling •  
Python Programming • EDA • Business Intelligence • Data Science Project Management

---




