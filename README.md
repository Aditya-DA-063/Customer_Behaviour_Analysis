# Customer Shopping Behavior Analysis

## Overview

This project focuses on understanding customer shopping behavior through data analysis and visualization. The aim is to identify purchasing patterns, compare customer segments, evaluate product performance, and understand how discounts, subscriptions, and shipping preferences relate to customer spending.

The project follows an end-to-end data analysis workflow, starting with data cleaning and exploratory data analysis in Python, followed by SQL-based business analysis, an interactive Power BI dashboard, and a presentation of the key insights and recommendations.

## Dataset

The dataset contains **3,900 purchase records and 18 columns**, covering customer demographics, product details, purchase history, and shopping preferences.

Key information includes:
- Customer demographics such as age, gender, and location
- Product categories, items purchased, and purchase amounts
- Subscription status and previous purchases
- Discounts, purchase frequency, and shipping type
- Customer review ratings and seasonal preferences

The dataset initially contained missing values in the review rating column, which were handled during data cleaning.

## Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Data preparation and exploratory data analysis |
| Pandas | Data cleaning, transformation, and feature engineering |
| Jupyter Notebook | Writing and documenting the analysis |
| SQL | Business queries and customer analysis |
| PostgreSQL | Database storage and SQL analysis |
| Power BI | Interactive dashboard and data visualization |
| PowerPoint | Presenting findings and business recommendations |

*Note: PostgreSQL is the database used in this project. The SQL queries can be adapted for MySQL or SQL Server where necessary.*

## Project Workflow

### 1. Data Loading and Exploration
- Imported the dataset into Python using Pandas.
- Examined the dataset structure, data types, and summary statistics.
- Checked for missing values and reviewed the available columns.

### 2. Data Cleaning and Preparation
- Handled missing review ratings using the median rating within each product category.
- Standardized column names using snake_case.
- Created customer age groups for demographic analysis.
- Converted purchase frequency categories into an approximate number of days.
- Checked for redundant columns and removed the duplicate promotional-code indicator.
- Prepared the cleaned dataset for database analysis.

### 3. SQL Business Analysis
Loaded the cleaned dataset into PostgreSQL and used SQL queries to investigate key business questions, including:

- How does revenue differ by gender?
- Which customers use discounts but still spend above the average?
- Which products have the highest average review ratings?
- How do purchase amounts compare across shipping types?
- How do subscribers and non-subscribers differ in spending and revenue?
- Which products have the highest percentage of discounted purchases?
- How can customers be classified as new, returning, or loyal?
- What are the top three products in each category?
- Are repeat buyers more likely to subscribe?
- Which age groups contribute the most revenue?

### 4. Power BI Dashboard
Built an interactive dashboard to present the analysis in a visual and easy-to-understand format. The dashboard helps explore customer purchasing patterns, product performance, revenue distribution, and subscription behavior.

### 5. Presentation and Recommendations
Prepared a PowerPoint presentation to communicate the main findings and potential business actions, making the analysis easier to understand for both technical and non-technical audiences.

## Dashboard

The Power BI dashboard focuses on the main areas explored during the analysis:

- Customer spending and revenue patterns
- Product ratings and purchasing preferences
- Subscriber versus non-subscriber behavior
- Customer loyalty and repeat purchases
- Discount usage and shipping preferences
- Revenue contribution across customer age groups

<img width="1197" height="677" alt="image" src="https://github.com/user-attachments/assets/e4b90af5-ffd5-4dfd-8908-7b0b3f24c8cc" />


## Key Findings and Business Recommendations

The analysis was used to explore customer behavior and develop recommendations in the following areas:

- **Subscription Growth:** Consider offering exclusive benefits to encourage more customers to subscribe.
- **Customer Loyalty:** Introduce rewards and targeted offers to encourage repeat purchases.
- **Discount Strategy:** Review discount usage to balance customer engagement with profitability.
- **Product Positioning:** Use product ratings and purchase trends to support marketing decisions.
- **Targeted Marketing:** Focus campaigns on relevant age groups and customer segments.
- **Shipping Preferences:** Use spending patterns across shipping types to inform delivery and promotional strategies.

These recommendations are intended to support better customer engagement and more informed business decisions.

## Project Structure

A suggested repository structure is:

```text
Customer-Shopping-Behavior-Analysis/
│
├── Customer_Shopping_Behaviour_Analysis.ipynb
├── customer_shopping_behavior.csv
├── sql_queries.sql
├── dashboard/
│   └── customer_shopping_behavior.pbix
├── presentation/
│   └── customer_shopping_behavior.pptx
├── images/
│   └── dashboard.png
└── README.md
```

*The folder structure is illustrative. Include the files and folders that are actually present in your repository.*

## How to Run

### Prerequisites
- Python 3.x
- Jupyter Notebook
- PostgreSQL and a database client
- Power BI Desktop

### Step 1: Clone the Repository

```bash
git clone <your-repository-url>
cd Customer-Shopping-Behavior-Analysis
```

### Step 2: Install Python Dependencies

```bash
pip install pandas sqlalchemy psycopg2-binary jupyter
```

### Step 3: Prepare the Dataset

Place `customer_shopping_behavior.csv` in the project directory, or update the file path in the notebook to match its location.

### Step 4: Run the Notebook

```bash
jupyter notebook
```

Open `Customer_Shopping_Behaviour_Analysis.ipynb` and execute the cells in order to explore, clean, and prepare the dataset.

### Step 5: Configure the Database

Create a PostgreSQL database and update the connection settings in the notebook with your database name, username, password, host, and port.

Run the database-loading section to transfer the cleaned dataset into PostgreSQL.

**Important:** Keep your database credentials private. Avoid committing passwords or other sensitive connection details to GitHub.

### Step 6: Execute SQL Queries

Open `sql_queries.sql` in your SQL editor, configure the database connection, and execute the queries to reproduce the business analysis.

### Step 7: Open the Dashboard and Presentation

Open the `.pbix` file in Power BI Desktop to explore the dashboard. Open the PowerPoint file to review the project findings and recommendations.

## Skills Demonstrated

- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Python and Pandas
- SQL Querying and Business Analysis
- Database Integration
- Customer Segmentation
- Data Visualization and Dashboard Development
- Business Insights and Reporting
- Presentation of Analytical Findings

## Conclusion

This project brought together Python, SQL, and Power BI to examine customer shopping behavior from multiple perspectives. It provided practical experience in preparing real-world-style data, translating business questions into SQL queries, presenting insights visually, and developing recommendations based on the analysis.

The project reflects the complete data analysis process, from working with raw data to communicating insights that can support business decisions.

---

**Author:** Aditya Suresh Panicker

**Focus:** Data Analytics | Python | SQL | Power BI
