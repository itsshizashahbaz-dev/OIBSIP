# 🧩 Task 3 — Unemployment Rate Analysis in India (KNIME)

## 🎯 Objective
The goal of this KNIME workflow is to analyze how unemployment rates in India changed during the COVID-19 pandemic.  
The analysis uses a **Bar Chart (Date vs Unemployment Rate)** to visually explore the impact of lockdowns on employment.

---

## 🧰 Tools Used
- **KNIME Analytics Platform**
- **CSV Dataset:** `Unemployment_Rate_upto_11_2020.csv`

---

## ⚙️ Steps to Run the KNIME Workflow

### 🪜 Step 1: Install and Launch KNIME
1. Download **KNIME Analytics Platform** from the [official KNIME website](https://www.knime.com/downloads).
2. Install the platform on your system (Windows, macOS, or Linux).
3. Launch KNIME and create a **New Workspace** to manage your workflows.

---

### 🪜 Step 2: Import the Workflow or Dataset
- If you have the **KNIME workflow file (.knwf)** or a **ZIP export**, import it into your workspace:
  - Go to **File → Import KNIME Workflow**.
  - Choose the workflow file or ZIP you created.
- If not, create your own workflow and use a **CSV Reader** node to load the file `Unemployment_Rate_upto_11_2020.csv`.
- Ensure **"Read column headers"** is checked and columns like `Date`, `Region`, and `Estimated Unemployment Rate (%)` are properly detected.

---

### 🪜 Step 3: Data Cleaning
1. Add a **Missing Value** node to handle null entries.
2. Add a **Duplicate Row Filter** node to remove duplicate records.
3. Optionally use a **Column Filter** node to keep relevant columns only:
   - `Date`
   - `Estimated Unemployment Rate (%)`

---

### 🪜 Step 4: Convert Date Column
- Use a **String to Date&Time** node to convert the `Date` column.
- Set the format to `dd-MM-yyyy` to ensure correct date parsing for visualization.

---

### 🪜 Step 5: Create the Bar Chart
- Add a **Bar Chart** node from the “Views” section.
- Configure the following settings:
  - **X-Axis:** `Date`
  - **Y-Axis:** `Estimated Unemployment Rate (%)`
- Optionally, group dates by month using a **GroupBy** node for smoother visualization.
- Customize colors and labels for clarity.

---

### 🪜 Step 6: Execute and View the Chart
- Right-click the **Bar Chart** node → **Execute and Open View**.
- Observe how unemployment rates change over time.
- The chart highlights a significant **spike during March–May 2020**, aligning with India's nationwide lockdown.

---

## 📊 Insights
- The unemployment rate rose drastically during the COVID-19 lockdown months.
- After May 2020, rates began to decline as restrictions eased.
- The bar chart clearly visualizes how employment was affected over time.

---

## 📁 Workflow Overview
### Nodes Used:
1. CSV Reader  
2. Missing Value  
3. Duplicate Row Filter  
4. String to Date&Time  
5. Column Filter (optional)  
6. Bar Chart  

---

## 💡 Advantages of Using KNIME
- **No Coding Required:** Intuitive drag-and-drop interface.
- **Reproducible Workflows:** Each step is visually documented.
- **Integration Flexibility:** Can combine Python, R, SQL, or Excel nodes.
- **Visualization Options:** Quick charting tools like bar charts, line plots, and scatter plots.
- **Easy Export:** Workflows can be shared as `.knwf` or `.zip` files.

---

## 🧾 Conclusion
This KNIME workflow demonstrates how to analyze and visualize unemployment data in a no-code environment.  
It highlights how India’s unemployment rate surged during the lockdown and later stabilized as restrictions were lifted.  
The project proves that even without programming, KNIME enables powerful, data-driven insights.

---
