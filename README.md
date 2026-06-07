# 🚖 NYC Taxi Trip Duration Prediction using LightGBM

A machine learning pipeline built to predict the duration of New York City taxi trips. Utilising **LightGBM**, this project processes over 1.4 million rows of raw spatial-temporal data, implementing feature engineering and 5 fold cross-validation strategy.

---

## 📈 Performance Summary
* **Evaluation Metric:** Root Mean Squared Log Error (RMSLE)
* **Mean 5-Fold CV RMSLE:** `0.3616`
* **Model Stability (Std Dev):** `± 0.0013`
* **Average Prediction Error (MAE):** `4.81` minutes

---

## 🚀 Key Engineering Highlights

* **Feature Extraction:** Engineered custom temporal features (`pickup_hour`, `pickup_day_of_week`, `is_weekend`) and spatial proxies (`manhattan_dist`) to mimic Manhattan's strict grid infrastructure.
* **Target Optimisation:** Applied a log-transformation to the target variable into a generalisable normal curve.
* **Production Validation:** Implemented a robust 5-Fold Cross-Validation loop to guarantee model stability across all unseen data slices.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Modeling Framework:** LightGBM
* **Data Engineering:** Pandas, NumPy
* **Evaluation & Splitting:** Scikit-Learn
* **Visualisation:** Matplotlib, Seaborn
