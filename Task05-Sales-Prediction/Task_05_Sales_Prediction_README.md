# 📊 Task 05 — Sales Prediction Using Machine Learning

## 🎯 Objective
The goal of this project is to predict **product sales** based on advertising budgets across different marketing platforms — **TV, Radio, and Newspaper**.  
The project compares two machine learning models — **Linear Regression** and **Random Forest Regressor** — to determine which model provides better prediction accuracy.

---

## 🧰 Tools & Libraries Used
- **Python 3.x**
- **Pandas** – Data manipulation and analysis  
- **NumPy** – Numerical operations  
- **Matplotlib & Seaborn** – Data visualization  
- **Scikit-learn (sklearn)** – Machine learning models and evaluation metrics  

---

## 📂 Dataset
**File Name:** `Advertising.csv`

### Dataset Description:
| Column | Description |
|--------|--------------|
| **TV** | Advertising budget spent on TV (in thousands of dollars) |
| **Radio** | Advertising budget spent on Radio |
| **Newspaper** | Advertising budget spent on Newspapers |
| **Sales** | Units of sales generated |

The dataset represents how advertising expenditure affects product sales.

---

## ⚙️ Steps to Run the Project

### 🪜 Step 1: Install Dependencies
Make sure the following libraries are installed in your Python environment:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

### 🪜 Step 2: Load and Explore the Dataset
- Import the dataset using `pandas.read_csv()`
- Check for missing values and understand column statistics using `.info()` and `.describe()`

---

### 🪜 Step 3: Prepare the Data
- Separate features (`X`) and target (`y`)
- Split the dataset into training and testing sets using `train_test_split()` (80–20 ratio)

---

### 🪜 Step 4: Train the Models

#### 🔹 Linear Regression
- Fit a **Linear Regression** model to learn the relationship between ad budgets and sales.  
- Predict sales on the test data and calculate metrics like:
  - **R² Score**
  - **Mean Absolute Error (MAE)**
  - **Root Mean Squared Error (RMSE)**

#### 🔹 Random Forest Regressor
- Train a **Random Forest Regressor** with 100 decision trees.
- Compare its performance with Linear Regression using the same metrics.

---

### 🪜 Step 5: Compare Model Performance
A DataFrame comparison shows both models side by side based on:
- R² Score (higher is better)
- MAE (lower is better)
- RMSE (lower is better)

Example Output:

| Model | R² Score | MAE | RMSE |
|--------|-----------|-----|------|
| Linear Regression | 0.89 | 1.21 | 1.56 |
| Random Forest | 0.97 | 0.55 | 0.80 |

---

### 🪜 Step 6: Visualize the Results
#### 1️⃣ **Actual vs Predicted Sales (Linear Regression)**
Scatter plot comparing actual and predicted values, with a reference line (`y = x`) showing perfect predictions.

#### 2️⃣ **Actual vs Predicted Sales (Random Forest)**
Similar scatter plot to visualize improvement in predictions.

#### 3️⃣ **Model Comparison (R² Score)**
A bar chart to visually compare both models based on their R² scores.

---

## 📊 Insights & Conclusion
- Advertising on **TV** had the strongest correlation with sales.  
- **Random Forest Regressor** outperformed Linear Regression in terms of prediction accuracy.  
- This model can be used by marketing teams to **optimize ad spend** and **forecast future sales** effectively.

---

## 🧾 Project Structure
```
📂 Task_05_Sales_Prediction
│
├── Advertising.csv
├── Task_05_Sales_Prediction.py
├── Task_05_Sales_Prediction_Report.docx
└── README.md
```

---

## 🏁 Final Thoughts
This project demonstrates how businesses can apply **machine learning** to real-world marketing data for better decision-making.  
By comparing multiple models, it highlights the importance of **model evaluation and selection** in data-driven analysis.
