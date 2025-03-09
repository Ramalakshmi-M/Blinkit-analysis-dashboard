# Blinkit Analysis Dashboard 📊
## Overview
This Power BI dashboard provides a detailed analysis of Blinkit grocery data, including sales trends, outlet performance, and product insights. The interactive dashboard helps in understanding sales distribution, outlet types, and customer preferences.

## Features 🚀
- **Total Sales Analysis** 💰
- **Item Category Performance** 📦
- **Outlet Establishment Trends** 🏬
- **Outlet Size & Location Impact** 📍
- **Interactive Filtering & Data Slicers** 🔍
- **KPI Cards for Key Metrics** 📊

---

## Steps Followed to Create the Dashboard 🛠️

### Step 1: Load Data into Power BI Desktop
- Imported the dataset from an Excel file (**BlinkIT Grocery Data.xlsx**).

### Step 2: Data Cleaning and Transformation
- Used **Power Query Editor** to preprocess data.
- Checked **column distribution, quality, and profile**.
- Ensured **column profiling** was based on the entire dataset.

### Step 3: Handling Missing Values
- Reviewed missing values in columns like **Item Weight** and **Item Visibility**.
- Applied transformations such as **filling missing values with averages** or **removing null entries**.

### Step 4: Created Calculated Columns & Measures
Added key **DAX measures**:
```DAX
Total Sales = SUM(BlinkIT_Grocery_Data[Sales])
Avg Sales = AVERAGE(BlinkIT_Grocery_Data[Sales])
No_of_Items = COUNT(BlinkIT_Grocery_Data[Item Identifier])
Avg Rating = AVERAGE(BlinkIT_Grocery_Data[Rating])
```

### Step 5: Designed the Dashboard Layout
- Used **yellow-themed sidebar** with **Blinkit logo**.
- Added **filter slicers** for:
  - `Item Type`
  - `Outlet Size`
  - `Outlet Location Type`

### Step 6: Created KPI Cards
Displayed key performance indicators using **Card Visuals**:
- **Total Sales**: `$1.20M`
- **Average Sales**: `$141`
- **Number of Items**: `8,523`
- **Average Rating**: `3.9`

### Step 7: Added Data Visualizations
- **Pie Chart**: Outlet Size Distribution
- **Bar Chart**: Total Sales by Item Type
- **Line Chart**: Outlet Establishment Trends (2012-2022)
- **Stacked Bar Chart**: Sales by Outlet Location (Tier 1, 2, 3)

### Step 8: Created Data Hierarchies
- Created a **hierarchical slicer** for **Item Type categories**.
- Segmented **Outlet Size** into (Small, Medium, High).

### Step 9: Published the Report
- Published the Power BI report to **Power BI Service** for sharing & collaboration.

---

## Insights from the Dashboard 📈
### Sales Trends
- **Supermarket Type 1** generated the highest sales (`$787.55K`).
- **Grocery Stores** had lower sales (`$151.94K`).

### Outlet Size & Location Impact
- **High-sized outlets** had the highest sales.
- **Tier 3 locations** contributed the most (`$472.13K`).

### Product Performance
- **Fruits & Vegetables** had the highest total sales (`$0.18M`).
- **Soft Drinks and Dairy Products** had moderate sales.

---

## How to Use This Repository
1. Clone the repository:
   ```sh
   git clone https://github.com/your-Ramalakshmi M/blinkit-analysis-dashboard.git
   ```
2. Open **BlinkIT Grocery Data.xlsx** in Power BI.
3. Load and clean the data using **Power Query Editor**.
4. Use **DAX measures** to analyze the data.
5. Explore the **dashboard visuals**.
6. Publish the report to **Power BI Service**.

## Technologies Used 🛠️
- **Power BI** 📊
- **DAX (Data Analysis Expressions)** 📑
- **Excel for Data Source** 📂

## Acknowledgments 🙌
Special thanks to **Blinkit** and **Power BI community** for resources and support!
