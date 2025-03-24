# 📦 Inventory Management System with Power BI

This project delivers an **Inventory Management System** using **Power BI**, designed to assist Warehouse and In-Plant Inventory Managers in efficiently managing inventory levels while ensuring optimal service levels.

---

## 🚀 **Project Overview**

The Inventory Management System provides actionable insights and data-driven decision-making to streamline inventory processes. It focuses on improving stock management, minimizing stockouts, and optimizing inventory turnover.

---

## 🛠️ **Tools & Technologies Used**

- **Power BI** – Data visualization and dashboard creation  
- **Excel** – Data preprocessing and manipulation  
- **SQL** – Data extraction and transformation  

**Dataset Source:**  
The dataset and project details are available on this [GitHub repository](https://github.com/Rahulshahu340/Inventory-Management_System.git).

---

## 📊 **Key Components of the Inventory Analysis Dashboard**

1. **ABC Classification** – Categorizes inventory based on importance and value to prioritize high-impact items.  
2. **XYZ Classification** – Groups inventory by demand variability, helping to manage demand fluctuations.  
3. **Inventory Turnover Ratio** – Measures how efficiently inventory is utilized.  
4. **Safety Stock Levels** – Maintains buffer stock to prevent stockouts.  
5. **Reorder Level Estimation** – Calculates reorder points and safety stock levels.  
6. **Average Weekly Demand** – Provides insights into demand patterns over time.  
7. **Stock Status** – Displays real-time inventory status to avoid overstocking or understocking.  
8. **Forecasting** – Predicts inventory needs for future periods, aiding in better planning.

---

## 📈 **Visualizations Used**

- **Stack Area Chart** – Visualizes averages and cumulative data for ABC classification.  
- **Cards, Gauges, and Slicers** – Showcase key metrics and filter requirements dynamically.  
- **Tables, Matrices, and Line Charts** – Present distribution trends, stock reports, and turnover ratios for in-depth analysis.  

---

## 🧠 **DAX Formulas & Advanced Analytics**

### 📌 **Sales Amount Calculation**

**DAX Formula:**

```DAX
Sales Amount = 
LOOKUPVALUE(
    Stock[Unit Price], 
    Stock[SKU ID], 
    'Weekly Demand Sheet'[SKU ID]
) * 'Weekly Demand Sheet'[Weeks Demand]
```

### 🔎 **Explanation:**

1. **LOOKUPVALUE(Stock[Unit Price], Stock[SKU ID], 'Weekly Demand Sheet'[SKU ID])**  
   - Retrieves the **Unit Price** from the `Stock` table by matching the `SKU ID` from the `Weekly Demand Sheet`.  
   - Ensures that the correct Unit Price is associated with the corresponding SKU.  

2. **Multiplication with 'Weekly Demand Sheet'[Weeks Demand]**  
   - Multiplies the retrieved Unit Price with the corresponding value in the **Weeks Demand** column.  
   - Computes the total sales amount based on weekly demand.  

### 📚 **Example:**

| SKU ID | Unit Price | Weeks Demand | Sales Amount |
|--------|------------|--------------|--------------|
| 101    | $10        | 5            | $50          |
| 102    | $20        | 3            | $60          |

---

## 🧩 **Advanced Functionalities**

- **Calculated Columns & Rows** – Perform date-based and conditional calculations.  
- **DAX Functions** – Enable complex calculations and data modeling.  
- **Forecasting Models** – Use historical data to predict future inventory requirements.

---

## 📌 **How to Use This Project**

1. Clone the repository from [GitHub](https://github.com/Rahulshahu340/Inventory-Management_System.git).
2. Open the Power BI file (`.pbix`) and load the dataset.
3. Analyze inventory data using the pre-built dashboard and modify it as needed.

---

## 📧 **Contact & Contribution**

Feel free to contribute to this project by submitting pull requests or reporting issues. For queries or suggestions, connect with me!

---

This structure makes your project more accessible, clear, and professional for GitHub documentation. Let me know if you’d like to make any changes or add more details! 😊
