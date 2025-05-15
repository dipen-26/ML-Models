Based on your provided dataset sample, here’s an updated and well-written `README.md` file tailored to your **Hotel Booking Status Prediction** project using K-Nearest Neighbors (KNN). This version reflects a human touch, with realistic assumptions drawn from the dataset structure.

---

# 🏨 Hotel Booking Status Prediction using KNN

## 📌 Objective

The aim of this project is to **predict whether a hotel booking will be canceled or not** using the **K-Nearest Neighbors (KNN)** classification algorithm. The model helps hotels proactively manage bookings, reduce last-minute cancellations, and optimize room availability.

---

## 📊 Dataset Overview

The dataset contains booking-related information such as guest details, reservation conditions, and customer preferences.

### 📁 Labels:

```text
Booking_ID,no_of_adults,no_of_children,no_of_weekend_nights,no_of_week_nights,type_of_meal_plan,
required_car_parking_space,room_type_reserved,lead_time,arrival_year,arrival_month,arrival_date,
market_segment_type,repeated_guest,no_of_previous_cancellations,no_of_previous_bookings_not_canceled,
avg_price_per_room,no_of_special_requests,booking_status
```

### 📌 Features Used for Prediction:

* **Numerical**:
  `no_of_adults`, `no_of_children`, `no_of_weekend_nights`, `no_of_week_nights`,
  `lead_time`, `arrival_month`, `arrival_date`, `avg_price_per_room`, `no_of_special_requests`, etc.

* **Categorical**:
  `type_of_meal_plan`, `room_type_reserved`, `market_segment_type`, `booking_status` (target)

* **Target Variable**:
  `booking_status` (`Canceled` or `Not_Canceled`)

---

## 🧹 Data Preprocessing

To prepare the data for training:

* **Categorical features** are encoded using **One-Hot Encoding**
* The **target variable** (`booking_status`) is **Label Encoded** (e.g., `Canceled = 1`, `Not_Canceled = 0`)
* **Numerical features** are **scaled** using StandardScaler to ensure all variables contribute equally to distance calculations

---

## 🧪 Model Training

* **Algorithm**: K-Nearest Neighbors (KNN) Classifier

* **Train-Test Split**:

  * 80% Training
  * 20% Testing
  * `random_state = 42` (for reproducibility)

* **Hyperparameter Tuning**:

  * Explored `k` values from **1 to 20**
  * Selected the `k` value that gave the **highest accuracy**

---

## 📈 Final Model Evaluation

The best model is:

* Trained using the optimal `k`
* Evaluated on the test set using **accuracy**, **confusion matrix**, and optionally **precision/recall/F1-score**

---

## 🎯 Prediction Goal

Predict whether a booking will result in:

* ✅ **Not\_Canceled**
* ❌ **Canceled**

This can help hotels:

* Better manage overbookings
* Improve resource planning
* Offer personalized retention strategies for likely-to-cancel guests

---

## 🛠️ Tools & Libraries

* Python
* pandas, numpy
* scikit-learn (for model training, preprocessing, evaluation)
* matplotlib / seaborn (for visualizations)

---

## ✅ Results

* Achieved optimal accuracy with tuned KNN
* Model makes reliable predictions on unseen data
* Balanced approach between model simplicity and predictive power

---

Let me know if you’d like this to include a **performance table**, **visual graphs**, or **code snippets** to enhance documentation further.
