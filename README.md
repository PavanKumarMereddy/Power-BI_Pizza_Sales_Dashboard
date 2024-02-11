# Power BI - Pizza Sales Dashboard

## Introduction
This project involves creating a sales dashboard using Power BI to analyze pizza sales data. The dataset contains various columns including `pizza_id`, `order_id`, `pizza_name_id`, `quantity`, `order_date`, `order_time`, `unit_price`, `total_price`, `pizza_size`, `pizza_category`, and `pizza_name`. The data was imported from a **PostgreSQL** database and underwent cleaning and transformation processes. The dashboard provides insights into sales performance, trends, and product analysis.

## Objective
The objective of this project is to create an interactive dashboard that enables users to visualize and analyze pizza sales data effectively. The dashboard should provide key metrics, trends, and insights to support decision-making processes for stakeholders.

## Project Steps

### 1.Data Import and Cleaning


![Screenshot 2024-02-11 104750](https://github.com/PavanKumarMereddy/Power-BI_Pizza_Sales_Dashboard/assets/155641231/f039ff5f-d726-490d-9c83-5496c6838d28)


- Imported data from PostgreSQL database.
*	Conducted data cleaning processes including:
+	Replacing values.
-	Updating table names.
*	Creating conditional columns.
+	Extracting year from the order_date column.

### 2.Data Modeling

![Screenshot 2024-02-10 103939](https://github.com/PavanKumarMereddy/Power-BI_Pizza_Sales_Dashboard/assets/155641231/34e3a95c-af5c-4b97-9f66-b4dfa0efcf9c)

+ Assembled the cleaned data into a single table for analysis.
*	Utilized DAX (Data Analysis Expressions) to create measures including

**Total revenue**
```
Total Revenue = SUM(pizza_sales[total_price])
```

**Total orders**
```
Total Orders = DISTINCTCOUNT(pizza_sales[order_id])
```

**Average order quantity**
```
Avg Pizza's Per Order = DIVIDE( [Total Pizza Sold],[Total Orders])
```

**Average order value**
```
Average Order Value = [Total Revenue]/[Total Orders]
```

**Total Pizzas Sold**
```
Total Pizza Sold = SUM(pizza_sales[quantity])
```



### 3.Data Visualization

+	Utilized various Power BI visuals including
*	Advanced card visuals for displaying key metrics.

![Screenshot 2024-02-11 110718](https://github.com/PavanKumarMereddy/Power-BI_Pizza_Sales_Dashboard/assets/155641231/12827998-5f59-4415-8ee8-0aecd8b35056)

+ Column chart to visualize orders by day.


![Screenshot 2024-02-11 110915](https://github.com/PavanKumarMereddy/Power-BI_Pizza_Sales_Dashboard/assets/155641231/0b8c8bf7-7e99-444b-8225-c816a2b752bb)

* Line chart to display monthly sales trend.

![Screenshot 2024-02-11 110932](https://github.com/PavanKumarMereddy/Power-BI_Pizza_Sales_Dashboard/assets/155641231/c44835eb-f5c9-4e32-8220-ef983b76f2e3)

* Donut charts to represent the percentage of orders by category and revenue.

![Screenshot 2024-02-11 110946](https://github.com/PavanKumarMereddy/Power-BI_Pizza_Sales_Dashboard/assets/155641231/b7841157-7a6d-49c1-9779-e2a3b8f2969e)      ![Screenshot 2024-02-11 111022](https://github.com/PavanKumarMereddy/Power-BI_Pizza_Sales_Dashboard/assets/155641231/c4976508-c5c4-401f-a8de-d73cf7266dce)




