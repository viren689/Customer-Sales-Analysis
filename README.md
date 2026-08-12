# Customer Sales Analysis

## 1. Project Overview

The Customer Sales Analysis project analyzes sales and customer data using Python and Pandas. The main objective is to understand customer purchasing patterns, identify high-value customers, analyze product and regional sales performance, study monthly and seasonal trends, and evaluate customer retention and churn.

The project demonstrates advanced data manipulation techniques in Pandas along with professional data visualizations and a sales performance dashboard.

---

## 2. Project Objectives

The main objectives of this project are:

* Analyze customer purchasing behavior.
* Identify the top customers based on revenue.
* Analyze sales performance by region.
* Identify the best-performing products.
* Analyze monthly and seasonal sales trends.
* Calculate customer lifetime value.
* Calculate customer retention and churn rates.
* Identify potential cross-selling opportunities.
* Create pivot tables for sales summarization.
* Create professional visualizations.
* Generate business insights and recommendations.

---

## 3. Technologies Used

* Python 3
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook
* Git and GitHub

---

## 4. Dataset Description

### Sales Dataset

The sales dataset contains 100 sales transactions and includes the following columns:

| Column      | Description                    |
| ----------- | ------------------------------ |
| Date        | Date of the sales transaction  |
| Product     | Product purchased              |
| Quantity    | Number of units purchased      |
| Price       | Price per unit                 |
| Customer_ID | Unique customer identifier     |
| Region      | Customer sales region          |
| Total_Sales | Total value of the transaction |

### Customer Dataset

The customer dataset contains 500 customer records and includes the following columns:

| Column           | Description                     |
| ---------------- | ------------------------------- |
| CustomerID       | Unique customer identifier      |
| Tenure           | Length of customer relationship |
| MonthlyCharges   | Monthly customer charges        |
| TotalCharges     | Total customer charges          |
| Contract         | Customer contract type          |
| PaymentMethod    | Customer payment method         |
| PaperlessBilling | Paperless billing status        |
| SeniorCitizen    | Senior citizen indicator        |
| Churn            | Customer churn status           |

---

## 5. Project Structure

```text
Week5-Customer-Sales-Analysis/
│
├── customer_analysis.ipynb
├── sales_data.csv
├── customer_data.csv
├── requirements.txt
├── README.md
├── analysis_report.pdf
│
└── screenshots/
    ├── data_exploration.png
    ├── monthly_sales.png
    ├── regional_sales.png
    ├── product_sales.png
    ├── top_customers.png
    ├── customer_churn.png
    └── dashboard.png
```

---

## 6. Setup Instructions

### Step 1: Install Python

Install Python 3 or later.

### Step 2: Download or Clone the Repository

Download this project or clone the GitHub repository.

### Step 3: Open the Project Folder

Open the project folder in VS Code or another Python development environment.

### Step 4: Install Required Libraries

Open the terminal and run:

```bash
pip install -r requirements.txt
```

### Step 5: Open the Notebook

Open:

```text
customer_analysis.ipynb
```

using Jupyter Notebook or VS Code.

### Step 6: Run the Analysis

Run the notebook cells from top to bottom.

---

## 7. Data Exploration

The datasets were explored before analysis to understand their structure and quality.

The following checks were performed:

* Number of rows and columns
* Column names
* Data types
* Missing values
* Duplicate records
* Statistical summary

The datasets contained no missing values or duplicate records, so no unnecessary missing-value replacement was required.

---

## 8. Data Cleaning and Preparation

The following preparation tasks were performed:

* Converted the sales `Date` column into datetime format.
* Converted numerical columns to appropriate numeric data types.
* Checked for missing values.
* Checked for duplicate records.
* Removed duplicate records where applicable.
* Standardized text values using Pandas string operations.

---

## 9. Feature Engineering

New features were created from the sales date:

* Year
* Month
* Month Name
* Quarter

A calculated sales column was also created using:

```text
Quantity × Price
```

The calculated sales value was compared with the existing `Total_Sales` column to validate the sales calculations.

---

## 10. Monthly Sales Analysis

Sales were grouped by year and month to calculate monthly revenue.

Multiple aggregation functions were used, including:

* Sum
* Mean
* Count

The analysis was used to identify changes in sales performance over time.

---

## 11. Customer Sales Analysis

Customer-level sales analysis was performed to identify valuable customers.

The following metrics were calculated:

* Total revenue
* Total quantity purchased
* Number of orders
* Average order value

The customers were ranked based on total revenue to identify the top customers.

---

## 12. Regional Sales Analysis

Sales performance was analyzed by region.

For each region, the project calculated:

* Total revenue
* Total quantity sold
* Number of orders
* Average order value

This helped identify the highest-performing sales region.

---

## 13. Product Performance Analysis

Products were analyzed based on:

* Total revenue
* Total quantity sold
* Number of orders
* Average sale value

This analysis was used to identify the best-performing products.

---

## 14. Multiple-Condition Filtering

Pandas conditional filtering was used to analyze specific sales transactions.

Both `AND` and `OR` conditions were implemented.

Examples included:

* High-value transactions
* Transactions from selected regions
* High-value transactions from selected regions

---

## 15. String Operations

Pandas string methods were used to clean and standardize text data.

The following operations were performed:

* Removing unnecessary spaces
* Standardizing product names
* Standardizing region names
* Cleaning customer IDs

Methods such as `.str.strip()` and `.str.title()` were used.

---

## 16. Dataset Merging

The sales and customer datasets were merged using the customer identifier.

A left join was used so that all sales transactions were retained while matching customer information was added where available.

The merged dataset was validated after the operation.

---

## 17. Pivot Table Analysis

Pivot tables were created using Pandas to summarize sales performance.

The analysis included:

* Sales by region and product
* Monthly sales by region

Pivot tables made it easier to compare sales performance across different categories.

---

## 18. Customer Churn and Retention Analysis

Customer churn was analyzed using the `Churn` column.

The following metrics were calculated:

* Total customers
* Retained customers
* Churned customers
* Retention rate
* Churn rate

This analysis provides insight into customer retention performance.

---

## 19. Customer Lifetime Value

Customer lifetime value was analyzed using the `TotalCharges` field from the customer dataset.

Customers were divided into:

* Low Value
* Medium Value
* High Value

The top customers based on lifetime value were also identified.

---

## 20. Cross-Selling Analysis

Customer purchase histories were analyzed to identify customers who purchased multiple products.

Product combinations were generated for customers with multiple product purchases.

These combinations can be used to identify potential cross-selling and product-bundling opportunities.

---

## 21. Seasonal Sales Analysis

Sales were grouped by quarter to identify seasonal patterns.

Quarterly analysis included:

* Total revenue
* Total quantity
* Number of orders
* Average order value

The highest-performing quarter was identified from the analysis.

---

## 22. Sales Performance Dashboard

A dashboard was created using Matplotlib containing five key visualizations:

1. Monthly Sales Trend
2. Sales by Region
3. Sales by Product
4. Top 10 Customers by Revenue
5. Customer Retention vs Churn

The dashboard provides a visual summary of the major findings from the analysis.

---

## 23. Business Insights

The analysis was used to identify:

* The highest-value customer.
* The best-performing sales region.
* The best-performing product.
* Monthly and seasonal sales patterns.
* Customer retention and churn levels.
* Customers purchasing multiple products.
* Potential cross-selling opportunities.

The exact results and values are available in the Jupyter Notebook and analysis report.

---

## 24. Business Recommendations

Based on the analysis, the following recommendations can be considered:

### Customer Retention

Focus retention campaigns on high-value customers and customers who may be at risk of churn.

### Regional Strategy

Use the strongest-performing region as a benchmark and investigate opportunities to improve lower-performing regions.

### Product Strategy

Continue promoting high-performing products while identifying opportunities to improve weaker products.

### Cross-Selling

Create product bundles and targeted recommendations based on frequently purchased product combinations.

### Customer Value

Provide personalized offers and loyalty benefits to high-value customers.

### Seasonal Planning

Plan inventory, promotions, and marketing campaigns around periods with stronger sales performance.

---

## 25. Testing and Validation

Several validation tests were performed to ensure the reliability of the analysis.

The project tested:

* Sales calculation accuracy
* Missing values
* Duplicate records
* Retention and churn calculations
* Revenue values
* Dataset merging

The validation results are available in the Jupyter Notebook.

---

## 26. Key Learning Outcomes

This project helped demonstrate practical skills in:

* Pandas data manipulation
* Data cleaning
* Data grouping and aggregation
* Multiple-condition filtering
* String operations
* Datetime processing
* Feature engineering
* Dataset merging
* Pivot tables
* Customer analysis
* Churn and retention analysis
* Data visualization
* Dashboard creation
* Business insight generation

---

## 27. Conclusion

The Customer Sales Analysis project demonstrates how Python and Pandas can be used to transform raw sales and customer data into meaningful business insights.

The project analyzed customer behavior, sales performance, regional trends, product performance, seasonal patterns, customer lifetime value, and retention. Advanced Pandas techniques such as grouping, aggregation, filtering, string operations, datetime processing, merging, and pivot tables were implemented throughout the analysis.

The resulting visualizations and dashboard provide a clear overview of sales performance and customer behavior. The insights generated from the analysis can support better decisions related to customer retention, product promotion, regional strategy, and cross-selling.

---

## 28. Author

**Viren Wankhade**

Data Science Intern

GitHub: `https://github.com/viren689`

