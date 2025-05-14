# 🔍 Optimizing Linear Regression Model to Predict Medical Insurance Charges

## 📌 Objective

The goal of this project is to **build and optimize a Linear Regression model** that accurately predicts a person’s **medical insurance charges** based on their demographic and health-related attributes.

### 🎯 Optimization Goals:

* Maximize **R² Score** for better prediction accuracy.
* Minimize **Mean Squared Error (MSE)** for lower prediction error.


## 📂 Dataset

* **File Used**: `insurance.csv`
* The dataset includes the following features:

  * **Age**
  * **Gender (Sex)**
  * **BMI (Body Mass Index)**
  * **Smoking Status**
  * **Number of Children**
  * **Region**
  * **Charges (Target Variable)**

### 🧮 BMI Categorization:

BMI values are categorized into:

* **Underweight**
* **Normal weight**
* **Overweight**
* **Obese**


## 🧪 Model Training & Testing

To ensure optimal performance of the model:

* Various **test sizes** are evaluated: `0.1`, `0.2`, `0.3`, `0.4`, `0.5`
* Multiple **random states** are tested: `1` to `49`

### 📊 Selection Criteria:

* Best model based on **maximum R² Score**
* Best model based on **minimum MSE**


## 🔍 Final Prediction

Using the optimized model, a prediction is made for the following new individual:

| Attribute | Value     |
| --------- | --------- |
| Age       | 34        |
| Gender    | Male      |
| BMI       | 26        |
| Children  | 3         |
| Smoker    | Yes       |
| Region    | Southwest |


## ✅ Outcome

* Identification of the most accurate Linear Regression model.
* Accurate prediction of insurance charges for new individual data.