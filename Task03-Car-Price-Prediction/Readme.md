# 🚗 Car Price Prediction (Internship Task 3)

## 📘 Overview
This project is part of my **Data Science Internship at Oasis Infobyte (AICTE)**.  
The goal was to develop a **machine learning model** to predict the **selling price of cars** based on their features such as brand, year, mileage, and fuel type.

---

## 🎯 Objective
To analyze car data and build predictive models that estimate car prices accurately using **Linear Regression** and **Random Forest Regressor**.

---

## ⚙️ Tools and Libraries
- **Python**
- **Jupyter Notebook / VS Code**
- **Libraries:** pandas, numpy, seaborn, matplotlib, scikit-learn

---

## 📊 Steps Performed
1. **Data Loading:** Loaded dataset using pandas.  
2. **Preprocessing:** Converted categorical features to numeric using one-hot encoding.  
3. **Train-Test Split:** Split data (80% training, 20% testing).  
4. **Model Training:** Trained Linear Regression and Random Forest models.  
5. **Model Evaluation:** Compared models using R², MAE, RMSE metrics.  
6. **Visualization:** Plotted Actual vs Predicted values and top 10 important features.

---

## 🧠 Why These Models?
- **Linear Regression:** A simple baseline model for understanding feature relationships.  
- **Random Forest:** A more powerful model capable of capturing non-linear dependencies for better accuracy.

---

## 📈 Results Summary
| Model | R² Score | MAE | RMSE |
|--------|-----------|-----|------|
| Linear Regression | ~0.60 | Moderate Error | Higher RMSE |
| Random Forest | ~0.85+ | Lower Error | Better Fit |

✅ **Best Model:** Random Forest Regressor

---

## 🔍 Key Insights
- Car price is strongly influenced by **Present Price**, **Car Age**, and **Fuel Type**.  
- Random Forest performed better due to its ability to handle non-linearity.  
- The feature importance plot revealed top contributors to car price prediction.

---

## 🏁 Conclusion
This project helped me strengthen my understanding of regression, feature engineering, and model evaluation.  
It also demonstrated how machine learning can solve **real-world pricing prediction problems** effectively.

---

