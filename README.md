📊 Retail Sales Performance Dashboard – Power BI

A complete end-to-end data analysis project built using Power BI, DAX, and Power Query to analyze retail sales, profit trends, segment performance, and top products.

📁 Project Files

Dashboard (PBIX file): Retail_Sales_Dashboard.pbix

Dataset (CSV): sample_superstore.csv

📌 Project Objective

To analyze the performance of a retail business across categories, regions, segments, and products. The dashboard helps identify:

High-performing categories

Profitability distribution

Regional trends

Yearly sales growth

Top-selling products

🛠️ Tools & Technologies Used

Power BI (Data modeling, DAX, Visualization)

Power Query (Data cleaning & transformation)

DAX Measures (KPIs: Total Sales, Profit Margin, Orders)

Excel/CSV Dataset (Sample Superstore Data)

📊 Key Insights

Technology category generated the highest sales (₹836K).

Office Supplies has the strongest profit margin (~17%).

West region performs strongly in both sales and profitability.

Furniture shows good sales but relatively lower profit margin.

There is a clear upward sales trend from 2014–2017.

Canon imageCLASS 2200 is the top-performing product.

▶️ Live Dashboard (Power BI Service)

https://app.powerbi.com/view?r=eyJrIjoiNWJiM2EzMzYtYzc3Zi00ODQxLWI0YjEtNGFiZWVlNTJiMjc2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9

📌 DAX Measures Used
Total Sales = SUM('sample_superstore'[Sales])

Total Profit = SUM('sample_superstore'[Profit])

Total Orders = COUNT('sample_superstore'[Order ID])

Profit Margin = DIVIDE([Total Profit], [Total Sales])

Cumulative Sales =
CALCULATE(
    [Total Sales],
    FILTER(
        ALL('sample_superstore'[Order Date]),
        'sample_superstore'[Order Date] <= MAX('sample_superstore'[Order Date])
    )
)

📈 Dashboard Features

KPI Cards (Sales, Profit, Orders, Profit Margin)

Line Chart (Sales trend over years)

Bar Charts (Category & Top Products analysis)

Map (Sales by State/Region)

Scatter Chart (Sales vs Profit by Sub-Category)

Donut Chart (Profit by Segment)

Interactive Slicers (Year, Region, Category)

📥 How to Use

Download the .pbix file

Open in Power BI Desktop

Use filters to explore the data

Review insights for decision-making

👩‍💻 About the Author

Aspiring Data Analyst with experience in Excel, Power BI, and ongoing training in SQL & Python (CodeBasics Bootcamp). Focused on building strong data visualization and storytelling skills.

⭐ If you liked this project

Feel free to ⭐ star this repository — it helps me grow as a data analyst!
