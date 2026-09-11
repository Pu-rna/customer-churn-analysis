# Customer Churn Analysis

## Project Overview

This project analyzes customer churn using customer, subscription, and support data stored in a SQLite database.

The objective is to understand customer churn patterns, calculate important business KPIs, explore customer behavior, and identify areas that may support customer retention strategies.

## Business Questions

- What is the overall customer churn rate?
- What is the customer retention rate?
- How does churn vary by plan type?
- How does churn vary by contract type?
- Does complaint frequency show a relationship with churn?
- Does customer satisfaction vary across churn groups?
- How much monthly revenue is associated with churned customers?
- What is the average customer tenure?
- What is the relationship between monthly charges and CLTV?

## Dataset

The analysis uses three tables:

- Customer
- Subscription
- Support

The final analysis contains 3,021 customers.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SQLite
- Jupyter Notebook

## Project Workflow

1. Data extraction from SQLite
2. Data inspection
3. Data cleaning
4. Data standardization
5. Missing-value handling
6. Feature engineering
7. Joining customer, subscription and support data
8. KPI analysis
9. Exploratory data analysis
10. Data visualization
11. Correlation analysis
12. Pivot table analysis
13. Business insights

## Data Cleaning

The project includes:

- Standardizing column names
- Converting date columns to datetime
- Standardizing gender values
- Standardizing plan and contract types
- Removing unnecessary columns
- Handling missing country values using existing state-country information
- Converting financial columns to numeric format
- Checking duplicate customer IDs
- Creating a churn flag from cancellation date
- Aggregating complaint information before merging support data

## Key KPIs

| KPI | Result |
|---|---:|
| Churn Rate | 34.46% |
| Retention Rate | 65.54% |
| Average Monthly Charges | ₹13.62 |
| Monthly Revenue at Risk | ₹13,261.03 |
| Average Customer Tenure | 882 days |
| Average Complaints per User | 1.60 |

## Analysis Performed

### Churn Analysis

Customer churn was analyzed across:

- Plan type
- Contract type
- State
- Gender
- Complaint frequency
- Customer satisfaction

### Exploratory Data Analysis

The project includes:

- Monthly churn trend
- Churn by plan type
- Churn by state
- Churn by gender
- Churn by contract type
- Churn by complaint count
- Churn by CSAT group
- Correlation heatmap
- Pairplot
- Multi-dimensional categorical analysis
- Pivot table analysis

## Key Findings

- The overall customer churn rate is 34.46%.
- The customer retention rate is 65.54%.
- Churned customers represent approximately ₹13,261 of monthly revenue at risk based on available monthly charge data.
- Average customer tenure is approximately 882 days.
- Customers have an average of 1.60 complaints per customer across the dataset.
- Complaint frequency does not show a clear relationship with customer churn in this dataset.
- Monthly charges and CLTV show a strong positive relationship.
- Churn patterns were further explored across plan type, contract type, gender, state, and customer satisfaction.

## Business Recommendations

- Identify customer segments with higher churn rates and investigate the underlying causes.
- Monitor customer satisfaction and support interactions as part of customer retention analysis.
- Prioritize retention efforts for high-value customers showing signs of churn.
- Review plan and contract segments with relatively higher churn.
- Consider developing a predictive churn model in a future phase.

## Future Improvements

- Build an interactive Power BI dashboard.
- Develop a machine learning model for churn prediction.
- Create customer-level churn risk segments.
- Perform deeper analysis of customer lifetime value and retention.

## Project Files

- `Churn_Analysis.ipynb` — Complete Python analysis
- `customer_churn.db` — SQLite database
- `exported_churn_data.csv` — Exported analysis dataset

## Author

Purna Kundu