# Marketing Analytics

## Project Overview
An online retail business is facing significant challenges with reduced customer engagement, declining conversion rates, high marketing expenses, and insufficient customer feedback analysis. This project aims to address these challenges by conducting an in-depth marketing analytics study using SQL, Python, and Power BI.

## Business Problems
1. **Reduced Customer Engagement**: The number of customer interactions and engagement with the website and marketing content has declined.
2. **Decreased Conversion Rates**: A smaller percentage of site visitors are converting into paying customers.
3. **High Marketing Expenses**: Marketing campaigns require substantial investment but fail to deliver the expected ROI.
4. **Need for Customer Feedback Analysis**: The business lacks insight into customer opinions about products and services, which is essential for improving engagement and conversions.

## Objectives
1. Analyze customer journeys and identify drop-offs at each stage.
2. Enrich datasets with geographical and sentiment analysis.
3. Identify patterns in customer engagement and conversions.
4. Provide actionable insights to improve marketing strategies and optimize expenses.

---

## Data Sources
- **SQL Server Database**:
  - `customers` table: Customer details.
  - `geography` table: Geographic data.
  - `customer_reviews` table: Product reviews.
  - `products` table: Product details.
  - `engagement_data` table: Customer engagement data.
  - `customer_journey` table: Data on customer actions and visits.

---

## Tools and Technologies Used
1. **Database Management**: SQL Server
   - Data extraction using SQL queries.
   - Data cleaning and transformations saved back to the database.
2. **Programming**: Python
   - Libraries: pandas, numpy, matplotlib, pyodbc, nltk.
   - Sentiment analysis using VADER (nltk).
   - Feature engineering and data processing.
3. **Visualization**: Power BI
   - Interactive dashboards to present insights.
   - Multiple slides focusing on different aspects of marketing analytics.
4. **Data Storage**:
   - Cleaned data exported to CSV files for ease of use in Power BI.

---

## Project Workflow

### 1. Data Extraction and Cleaning
- Established a connection to SQL Server using `pyodbc`.
- Loaded multiple tables into Pandas DataFrames using SQL queries.
- Performed the following data cleaning steps:
  - Merged customer and geography data for enriched analysis.
  - Categorized products based on price range.
  - Standardized and normalized engagement data.
  - Removed duplicate records from customer journey data.
  - Imputed missing values with meaningful defaults (e.g., average duration).

### 2. Sentiment Analysis
- Applied VADER sentiment analysis to customer reviews.
- Calculated compound sentiment scores and categorized reviews as Positive, Negative, Neutral, or Mixed.
- Buckets were created for sentiment score ranges (e.g., `-1.0 to -0.5`).

### 3. Data Export
- Cleaned datasets were exported as:
  - `cleaned_engagement.csv`
  - `cleaned_reviews.csv`
  - `cleaned_product.csv`
  - `cleaned_customer_geography.csv`
  - `cleaned_customer_journey.csv`

### 4. Visualization
Created a series of interactive Power BI dashboards:
1. **Engagement Insights**: Metrics such as views, clicks, and content performance.
2. **Product Performance Analysis**: Sales and customer feedback for various product categories.
3. **Customer Journey Analytics**: Funnel analysis and average journey durations.
4. **Customer Sentiment Analysis**: Sentiment trends and distribution by product and geography.

---

## Key Insights
1. **Customer Engagement**:
   - Identified peak engagement periods and underperforming content types.
2. **Conversion Rates**:
   - Highlighted stages where significant drop-offs occur.
3. **Customer Feedback**:
   - Unveiled key pain points and positive drivers through sentiment analysis.
4. **Geographic Patterns**:
   - Pinpointed regions with high/low conversion rates and engagement levels.

---

## Repository Structure
```
Marketing_Analytics/
|-- marketing_analytics.ipynb              # Python scripts for data cleaning and analysis
|-- marketing_analytics_dashboard.pbix          # PBIX files for Power BI visualizations
|-- Cleaned Data/
|   |-- Cleaned Data csv files                 # Processed datasets ready for analysis
|-- Database/
|   |-- Marketing Data.bak               # SQL database backup file
|-- README.md                    # Project documentation
|-- marketing_analytics_ppt.pptx        
```

---

## How to Use This Repository
1. Clone the repository to your local system.
   ```
   git clone https://github.com/vms003/Marketing_Analytics.git
   ```
2. Set up a SQL Server database with the provided schema and data.
3. Run the Python scripts to clean and analyze the data.
4. Open the Power BI dashboard files (`.pbix`) to explore insights interactively.

---

## Authors
**Viraj Suthar**  
*Data Analyst | Data Scientist | Business Intelligence Enthusiast*  
[Email](mailto:virajsuthar2003@gmail.com) | [LinkedIn](https://www.linkedin.com/in/viraj-suthar-517445333/)

