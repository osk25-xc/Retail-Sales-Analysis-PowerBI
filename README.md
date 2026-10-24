# 📊 Retail Sales Analysis — Power BI Dashboard

An interactive **Retail Sales Analysis Dashboard** built using Microsoft Power BI to analyze sales performance, profitability, regional trends, and product performance.

## 🎯 Project Objective

The objective of this project is to analyze retail sales data and turn it into meaningful business insights that can support better decision-making.

## 🛠️ Tools & Technologies

- **Power BI Desktop** — Dashboard development and visualization
- **Power Query** — Data cleaning and transformation
- **DAX** — Measures and KPI calculations
- **Microsoft Excel / CSV** — Dataset and data source

## 📈 Dashboard Features

- **Total Sales** — Overall sales performance
- **Total Profit** — Business profitability
- **Total Orders** — Unique order count
- **Profit Margin %** — Profitability as a percentage of sales
- **Sales Trend** — Daily sales performance over time
- **Sales by Category** — Category-wise sales comparison
- **Sales by Region** — Regional performance analysis
- **Top 10 Products** — Best-performing products by sales
- **Interactive Slicers** — Filter the dashboard by date, region, and category

## 📐 Key DAX Measures

### Total Sales
```dax
Total Sales = SUM('Retail_Sales_Analysis_Dataset'[Sales])
```

### Total Profit
```dax
Total Profit = SUM('Retail_Sales_Analysis_Dataset'[Profit])
```

### Total Orders
```dax
Total Orders = DISTINCTCOUNT('Retail_Sales_Analysis_Dataset'[Order ID])
```

### Profit Margin %
```dax
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
```

## 📂 Project Files

- `Retail_Sales_Analysis.pbix` — Power BI dashboard
- `Retail_Sales_Analysis_Dataset.csv` — Dataset in CSV format
- `Retail_Sales_Analysis_Dataset.xlsx` — Dataset in Excel format

## 🚀 How to Use

1. Download or clone this repository.
2. Open `Retail_Sales_Analysis.pbix` using Power BI Desktop.
3. If prompted, update the dataset file path to the downloaded CSV or Excel file.
4. Refresh the data if required.
5. Explore the dashboard using the available charts and slicers.

## 💡 Business Insights

This dashboard can help users:

- Compare sales performance across regions and product categories.
- Identify top-performing products.
- Monitor profitability and profit margins.
- Explore sales trends over time.
- Support data-driven retail business decisions.

## 👨‍💻 Author

**Omkar S. Kshirsagar**

Aspiring Data Analyst | SQL | Python | Excel | Power BI

- GitHub: [osk25-xc](https://github.com/osk25-xc)
- LinkedIn: [Omkar S. Kshirsagar](https://www.linkedin.com/in/omkar-s-kshirsagar-07298b2b1/)

---

⭐ If you find this project useful, feel free to star this repository.
