# 🍷 Wine Quality Prediction

A machine learning project to predict the **quality of wine** using physicochemical properties such as acidity, sugar content, pH, and alcohol. The dataset includes red wine samples with a quality score (0-10) rated by wine tasters.


## 📊 Problem Statement

Given physicochemical tests of red wine samples, predict the **wine quality score** using regression techniques.


## 📁 Dataset Overview

The dataset contains the following **12 features** for each wine sample, along with a target `quality` score:

| Feature                 | Description                                                        |
|-------------------------|--------------------------------------------------------------------|
| `fixed acidity`         | Tartaric acid content (g/dm³)                                      |
| `volatile acidity`      | Acetic acid content – too much can cause unpleasant taste         |
| `citric acid`           | Adds freshness and flavor                                          |
| `residual sugar`        | Sugar remaining after fermentation (g/dm³)                         |
| `chlorides`             | Salt content                                                       |
| `free sulfur dioxide`   | SO₂ in free form — protects wine from microbial growth             |
| `total sulfur dioxide`  | Total SO₂ present                                                  |
| `density`               | Density of wine — related to sugar and alcohol content             |
| `pH`                    | Acidity level (lower is more acidic)                              |
| `sulphates`             | Sulfates added to enhance wine shelf life                          |
| `alcohol`               | Alcohol percentage (%)                                             |
| `quality`               | Target variable — wine quality score (integer between 0 and 10)    |
| `Id`                    | Unique identifier for each sample                                  |


## 🧠 Machine Learning Model

This project uses **Linear Regression** to predict the wine quality. The model was trained using Scikit-learn.

### 🔧 Model Metrics

- **Mean Squared Error (MSE):** ~0.38  
- **Interpretability:** Coefficients show how much each feature affects quality prediction


## 📈 Example Output

After training the model:

- **Predicted Quality:** `5.80`  
- **Real Quality:** 5 or 6 (approximate — prediction within good range)


## 🧪 Sample Prediction

```python
new_sample = np.array([[8, 0.4, 0.40, 15, 0.048, 40, 150, 0.99, 3, 0.45, 10.5]])
predicted_quality = model.predict(new_sample)
