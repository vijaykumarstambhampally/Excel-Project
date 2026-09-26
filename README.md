# 🚲 Bike Sales Analysis & Interactive Dashboard

An end-to-end Excel data analysis project using the **Bike Buyers Dataset** from Kaggle. This project transforms raw customer data into clean, structured sheets, builds automated pivot tables, and visualizes insights on an interactive Excel dashboard.

---

## 📌 Project Overview
The goal of this analysis is to evaluate customer demographic features—such as income level, commute distance, age group, marital status, education, and region—to identify key factors driving bicycle purchasing decisions.

---

## 📂 Repository Structure
* **`Excel Dashboard.xlsx`**: The main Excel workbook containing the full workflow across dedicated tabs:
  * **`bike_buyers`**: Original raw dataset sourced from Kaggle.
  * **`Work Sheet`**: Cleaned and transformed dataset.
  * **`Pivot Table`**: Calculated summary metrics and aggregated tables.
  * **`DashBoard`**: Interactive dashboard with charts and slicers.

---

## 🛠️ Data Processing & Analysis Workflow

### 1. Data Cleaning & Transformation (`Work Sheet`)
* **Standardization:** Normalized categorical values (e.g., converted single-character values like `M`/`S` in Marital Status and `M`/`F` in Gender to `Married`/`Single` and `Male`/`Female` for clarity).
* **Data Formatting:** Applied standard currency formatting to `Income` and removed duplicates.
* **Age Brouting / Binning:** Created a nested `IF` condition / formula column (`Age Brackets`) categorizing customers into age ranges:
  * **Adolescent** (`< 31`)
  * **Middle Age** (`31 - 54`)
  * **Old** (`>= 55`)

### 2. Pivot Table Aggregations (`Pivot Table`)
* Calculated average income per bike purchase split by gender.
* Summarized purchase counts across different age brackets.
* Analyzed customer commute distance against bicycle buying patterns.

---

## 📊 Dashboard Visualizations (`DashBoard`)

The main dashboard consolidates key insights into visual representations:
1. **Average Income per Purchase (Bar Chart):** Compares income levels between buyers and non-buyers across genders.
2. **Customer Age Brackets (Line Chart):** Analyzes bike purchases across Adolescent, Middle Age, and Old age categories.
3. **Customer Commute Distance (Line Chart):** Evaluates how commute length (0-1 Miles, 1-2 Miles, 2-5 Miles, 5-10 Miles, 10+ Miles) impacts bike buying trends.
4. **Interactive Filters (Slicers):**
   * **Marital Status** (`Married`, `Single`)
   * **Region** (`Europe`, `North America`, `Pacific`)
   * **Education** (`Bachelors`, `Graduate Degree`, `High School`, `Partial College`, `Partial High School`)

---

## 💡 Key Insights & Observations
* **Income Impact:** Male and female customers who purchased bikes had a higher average income compared to those who did not.
* **Peak Age Demographic:** Middle-aged individuals (31–54 years old) represent the highest volume of bike buyers.
* **Commute Dynamics:** Customers living closer to their workplace (0–1 miles) show higher purchase rates, whereas purchase frequency declines for longer commutes.

---

## 🚀 How to View and Use
1. Download or clone `Excel Dashboard.xlsx` from this repository.
2. Open the file in **Microsoft Excel**.
3. Navigate to the **`DashBoard`** tab and interact with the **Slicers** on the left to filter metrics dynamically by region, education level, and marital status.
