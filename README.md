# 🌧 Rainfall Prediction Using Machine Learning

This project analyzes weather data to predict *whether it will rain tomorrow* using machine learning models. It includes complete steps from data cleaning and visualization to model evaluation and feature importance analysis.

---

## 📁 Dataset

- *Name*: weatherAUS.csv
- *Source*: [Australian Bureau of Meteorology](https://www.kaggle.com/jsphyg/weather-dataset-rattle-package)
- *Rows*: ~145,460
- *Columns*: 24 weather attributes (temperature, humidity, wind, etc.)
- *Target*: RainTomorrow (Yes/No)

---

## 📊 Project Workflow

1. *Missing Data Analysis*
   - Visualized missing values as bar and pie charts.
   - Dropped columns with excessive missing data.
   - Removed rows with nulls.

2. *Data Visualization*
   - Plotted distributions of rainfall, humidity, pressure, and temperature.
   - Analyzed target variable and class imbalance.

3. *Feature Engineering*
   - Dropped irrelevant columns: Date, Location, Sunshine, etc.
   - Label encoded categorical variables.

4. *Correlation Analysis*
   - Correlation heatmap to analyze relationships between features.

5. *Model Training*
   - Trained three classifiers:
     - 🌲 *Random Forest*
     - 🌳 *Decision Tree*
     - 📈 *Logistic Regression*
   - Split data (80% training, 20% testing)
   - Scaled features using StandardScaler

6. *Model Evaluation*
   - Accuracy, confusion matrix, precision, recall, F1-score.
   - Visual comparison of all models.

7. *Feature Importance*
   - Identified top contributing features from the Random Forest model.

---

## 🔍 Best Model

🏆 *Random Forest Classifier*  
- Highest accuracy among all models
- Top features included:
  - Humidity3pm
  - Rainfall
  - Pressure9am
  - Temp3pm
  - MaxTemp

---

## 📂 Files in Repository

| File                          | Description                             |
|------------------------------|-----------------------------------------|
| rainfall_prediction.ipynb  | Jupyter Notebook with full analysis     |
| weatherAUS.csv             | Weather dataset (if included)           |
| README.md                  | Project overview (this file)            |

---

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/Rainfall-Prediction-ML.git
   cd Rainfall-Prediction-ML
