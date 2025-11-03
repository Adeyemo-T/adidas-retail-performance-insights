# ADIDAS Commercial Performance Analysis: Optimizing Profitability and Retailer Strategy

![Image](https://github.com/user-attachments/assets/2442d22b-9f0e-4cfa-af2a-40e859bc1fb3)

## Project Background

A major sportswear brand (ADIDAS) requires a comprehensive commercial performance review to optimize its distribution strategy, maximize profitability across its retail partners, and address regional sales imbalances. The challenge is to identify which retailers and regions are the most profitable, not just in terms of sales volume, but Operating Margin.

This project delivers a complete overview of the commercial performance data to inform decisions on inventory allocation, retailer partnerships, and product focus.

Insights and recommendations are provided on the following key areas:
* **Profitability & Sales Trend Analysis:** Evaluation of the monthly trend for Sales and Operating Margin.
* **Retailer Performance Benchmarking:** Comparison of sales, profit, and margin across major retail partners (e.g., Walmart, Foot Locker).
* **Regional and Product Performance:** Analysis of sales distribution by region and profitability breakdown by product category.


* **Interactive Dashboard:** The full Commercial Performance dashboard can be accessed [here](https://app.powerbi.com/MobileLandingPage?ctid=9db3791d-d5d0-4f91-b691-e83929715f73&pbi_source=linkShare&action=OpenLink&linkId=gG5NN6FnJY).

## Data Structure & Initial Checks

#### Data Overview
The analysis was built on a **Star Schema** data model developed within Power BI. The data was sourced from a single large transactional file which was logically segmented and modeled into two key tables:
* **'Data Sales Adidas' (Fact Table):** Contains transactional data including Sales, Operating Profit, Price per Unit, Product, Region, and Retailer.
* **'Date Table' (Dimension Table):** Contains hierarchical time attributes (Date, Year) used for filtering and calculating monthly trends.

#### Data Model (Star Schema)
The tables are connected via a **One-to-Many relationship** between the `Date Table` (one side) and the `Data Sales Adidas` table (many side) on the `Date` or `Invoice Date` field. This structure allows for accurate time-intelligence calculations.


*(**Action:** Insert an image of your Power BI Model View showing the two connected tables.)*

#### Data Cleaning and Preparation
The data cleaning and transformation process was entirely executed using **Power Query (M Language)** to ensure data quality and integrity before modeling and visualization.

* **Fact Table Transformation:** Power Query was used to handle missing values and correct data types for currency and numerical fields.
* **Dimensional Table Creation:** A dedicated **'Date Table'** was created and standardized to ensure consistent time intelligence.
* **Key Metric Calculation (DAX):** Measures like **Sales**, **Operating Profit**, and **Operating Margin** were calculated in Power BI using DAX (Data Analysis Expressions).

## Executive Summary

The overall commercial performance is strong, with total **Sales reaching $899.9 million** and an **Operating Margin of 37%**. However, analysis reveals severe profitability disparities across retailers and a concentration of low-margin sales in specific product lines. The primary strategic focus must be shifting resources away from **underperforming retailers (Walmart, Kohl's)** and mitigating the risk posed by low-profitability products like **Women's Athletic Footwear** to secure future profitability.


#### Overview of Commercial Performance

This section presents the high-level financial health and sales trend, showing the foundation of the commercial operation.

![Image](https://github.com/user-attachments/assets/e5ed065f-8aed-4f19-a255-44d78a52a161)



#### Retailer Profitability & Performance

* **Leading Retailers:** **Foot Locker and West Gear** are the clear leaders, generating both the highest sum of Operating Profit and strong Operating Margins.
* **Underperforming Risks:** **Walmart and Kohl's** show the lowest Operating Margins, requiring immediate negotiation or strategic re-evaluation of partnership terms.

![Retailer Performance Bar Chart](YOUR_IMAGE_LINK_FOR_RETAILER_PERFORMANCE_CHART_HERE)
*(**Action:** Insert the image link showing the **"Retail Giants Leading the Profit Race"** bar chart and the **Underperforming Retailers table**.)*



#### Product & Regional Profit Breakdown

* **Top Selling Products:** **Men's Athletic Footwear and Women's Apparel** are the top-selling product categories.
* **Low Profit Risk:** Products like **Women's Athletic Footwear** have high sales but contribute lower Operating Profit, indicating a need to investigate their cost structure.
* **Regional Concentration:** The **Northeast and West** regions dominate sales distribution.

![Product and Regional Sales Breakdown](YOUR_IMAGE_LINK_FOR_PRODUCT_AND_REGIONAL_CHARTS_HERE)
*(**Action:** Insert the image link showing the **Regional Sales Distribution Map** and the **Products with Low Profitability** table.)*

## Business Recommendations

Based on the detailed commercial performance analysis, the following actions are critical to improve overall operating margin and strategically allocate resources:

* **1. Renegotiate or Exit Low-Margin Retailers:** Immediately review partnership agreements with **Walmart and Kohl's**. The recommendation is to either **negotiate higher wholesale prices** or strategically **reduce inventory allocation** to these partners.
* **2. Prioritize Top-Tier Retailers:** Increase inventory allocation and marketing support for top-performing partners like **Foot Locker and West Gear**.
* **3. Product Profitability Review:** Launch an investigation into the cost structure of **Women's Athletic Footwear** and **Men's Street Footwear** due to their low contribution to Operating Profit.
* **4. Focus on High-Profit Regions:** Prioritize marketing spend and distribution resources in the dominant **Northeast and West** regions.
* **5. Strategic Inventory Shift:** Reduce the production or import of low-profitability product lines and **reallocate those manufacturing resources** toward higher-profit, high-demand items.
