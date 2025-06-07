# 🧮 Sales Revenue Analysis with Excel Power Pivot & DAX

This project showcases an Excel-based data analysis pipeline using **Pivot Tables,** **Power Pivot** and **DAX formulas**. The goal is to analyze sales performance and revenue patterns for a wholesale company dealing in six core products.

## 📁 Repository Contents

- **`sales_data.xlsx`**  
  Contains the raw source data (hidden by default—see below to access).
  
- **`Sales_Analysis_DAX_Model.xlsx`**  
  Includes multiple pivot tables, edited Power Pivot, and DAX-based calculations for deep revenue analysis.

---

## 🔍 How to View the Source Data

When opening `sales_data.xlsx`, the worksheet appears empty. To view and interact with the Power Pivot source data:

1. Go to the **Power Pivot** tab on the Excel toolbar.
2. Click **Manage**.
3. The data will be on the newly opened page.

**Plesae follow the same steps above when viewing the edited Power Pivot that includes 'cost, price, gross revenue, tax, and total revenue' on 'Sales_Analysis_DAX_Model.'**

---

## 🛒 About the Dataset

The dataset represents wholesale order data for the following products:
- Basil
- Garlic
- Jalapeno
- Lemon
- Mandarin
- Rosemary

Each row of the dataset includes:
- `OrderID`
- `StoreID`
- `OrderDate`
- `OrderYear`
- `OrderMonth`
- `Product`
- `Quantity`
- `Cost` (to manufacture)
- `Price` (selling price = 1.75 × cost)
- `Gross Revenue` (price × quantity)
- `Tax` (5% if quantity > 15, else 12%)
- `Total Revenue` (gross revenue + tax)

---

## 📊 Pivot Tables & DAX Measures

The `Sales_Analysis_DAX_Model.xlsx` contains the following pivot tables and DAX-powered insights:

### ✅ 1. Total Sales (< 10 Quantity)
**Sheet:** `Total Sales<10 PT`  
- Shows total revenue from orders with **quantities less than 10**.
- Created using a custom DAX filter measure with `SUMX()` and `FILTER()` functions.

### 📈 2. Aggregate Total Revenue
**Sheet:** `TotalSalesAggPT`  
- Displays the **total revenue** across the entire dataset.
- Uses a basic `SUM()` function on the total revenue column.

### 📊 3. Average Tax by Product
**Sheet:** `Average Order Tax by Product PT`  
- Shows **average tax per order**, grouped by **product**.
- Uses the `AVERAGE()` DAX function.

### 📆 4. Yearly Total Revenue
**Sheet:** `Total Revenue PT`  
- Displays **total revenue by year**.
- Useful for understanding sales trends over time.

---

## 📌 Key DAX Concepts Used

- `SUMX()`, `FILTER()` for conditional aggregations
- `CALCULATE()` for custom measure evaluation context
- `AVERAGE()` for aggregating tax by product
- Logical and arithmetic operations for revenue/tax computation

---

## 🚀 Getting Started

To explore the analysis:

1. Download and open `Sales_Analysis_DAX_Model.xlsx`.
2. Review the pivot tables in each sheet listed above.
3. If needed, access the raw data through the Power Pivot model (see above).

---

## 📚 Learning Goals

- Mastery of Power Pivot and DAX for Excel-based data modeling
- Understanding of calculated columns vs. measures
- Revenue computation workflows (cost, price, tax, gross and net revenue)
- Applying business logic with conditional DAX

---

## 🧠 Future Improvements

- Automate tax rate rules via a lookup table
- Integrate slicers for interactive filtering by product/year
- Export insights to Power BI for dashboard visualizations

---

## 📩 Questions?

If you have questions, suggestions, or want to collaborate, feel free to open an issue or contact me!
