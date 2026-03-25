# 🏠 House Price Prediction Model Evaluation Report

## 📌 Objective

The objective of this project is to build a machine learning model to predict house prices based on features such as area, bedrooms, bathrooms, property age, location, and property type.

---

## 📊 Dataset Description

The dataset contains the following features:

* **Area** – Size of the house (in sq.ft)
* **Bedrooms** – Number of bedrooms
* **Bathrooms** – Number of bathrooms
* **Age** – Age of the property (in years)
* **Location** – Geographic location of the property
* **Property_Type** – Type of property (e.g., Apartment, Villa)
* **Price** – Target variable (house price)

Irrelevant columns such as `Property_ID` were removed during preprocessing.

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

* Removed unnecessary column: `Property_ID`
* Handled missing values by dropping null entries
* Converted categorical variables (`Location`, `Property_Type`) using one-hot encoding
* Split the dataset into training (80%) and testing (20%) sets

---

## 🤖 Models Implemented

The following machine learning models were used:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor

---

## 📏 Evaluation Metrics

Model performance was evaluated using:

* **MAE (Mean Absolute Error)** – Measures average prediction error
* **MSE (Mean Squared Error)** – Penalizes larger errors
* **R² Score (Coefficient of Determination)** – Measures model accuracy

---

## 📈 Model Performance

| Model             | MAE     | MSE           | R² Score |
| ----------------- | ------- | ------------- | -------- |
| Linear Regression | 2188736 | 8454330868276 | 0.94     |
| Decision Tree     | 2280000 | 9164761041666 | 0.94     |
| Random Forest     | 1493949 | 4120314726645 | **0.97** |

---

## 📊 Visualization

A scatter plot of **Actual vs Predicted Prices** was created to evaluate model performance:

* Points closer to the diagonal line indicate better predictions
* Random Forest shows tighter clustering, indicating higher accuracy

---

## 🔍 Feature Importance

Based on the Random Forest model, the most influential features were:

* **Area**
* **Location**
* **Bedrooms**
* **Property Type**

These features significantly impact house price predictions.

---

## 🏆 Best Model

The **Random Forest Regressor** performed the best:

* Highest R² Score (**0.97**)
* Lowest MAE and MSE
* Better handling of complex and non-linear relationships

---

## 💡 Key Insights

* Larger houses generally have higher prices
* Location plays a crucial role in determining house value
* More bedrooms and bathrooms increase the property price
* Tree-based models outperform linear models for this dataset

---

## 📌 Conclusion

The project successfully developed a machine learning model for house price prediction. Among all models, the Random Forest Regressor provided the most accurate and reliable results.

---

## 🚀 Future Scope

* Perform hyperparameter tuning for better accuracy
* Include additional features (e.g., amenities, nearby facilities)
* Deploy the model using Streamlit for real-time predictions
* Use larger datasets for improved generalisation

---
