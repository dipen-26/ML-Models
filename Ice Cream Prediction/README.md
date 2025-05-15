# 🍦 Predicting Ice Cream Sales Using Polynomial Regression

## 📌 Objective

The goal of this project is to **predict ice cream sales based on temperature** using **Polynomial Regression**, and to determine the best-fit model by testing polynomial degrees from 1 to 5.

### 🎯 Optimization Goals:

* Identify the **best polynomial degree** that provides a balance between **model complexity and accuracy**.
* Maximize the **R² Score** to evaluate prediction performance.


## 📂 Dataset

* **Features Used**:

  * `Temperature (°C)`
  * `Ice Cream Sales (units)`

* **Sample Data**:

  ```text
  Temperature (°C), Ice Cream Sales (units)
  -4.66,              41.84
  -4.31,              34.66
  -4.21,              39.38
  -3.95,              37.54
  ```

* **Target Variable**:

  * `Ice Cream Sales (units)`


## 🧪 Model Training & Testing

* **Train-test split**:

  * `80%` training
  * `20%` testing
  * Using `random_state = 20` for reproducibility

* **Model Evaluation**:

  * Polynomial degrees tested: `1` to `5`
  * Best model chosen based on **maximum R² Score** on test data


## 🔍 Final Prediction

After identifying the best-performing polynomial degree, the model is retrained and used to predict ice cream sales at:

* **Temperature**: `4°C`


## ✅ Outcome

* Best polynomial degree is selected based on evaluation.
* Accurate prediction of ice cream sales at a specific temperature.
