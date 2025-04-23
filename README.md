
# 📊 Marketing Analytics Portfolio Project


## 📌 Business Case

An online retail business is facing reduced customer engagement and conversion rates despite launching several new online marketing campaigns. The business has identified the need for a comprehensive data-driven analysis to identify weaknesses in their marketing strategies and uncover improvement opportunities.

**Key Challenges:**
- **Reduced Customer Engagement:** Drop in user interaction with marketing content.
- **Decreased Conversion Rates:** Fewer website visitors are making purchases.
- **High Marketing Expenses:** Increased spending without proportional returns.
- **Need for Customer Feedback Analysis:** Insights from reviews and social media are essential to enhance engagement and conversions.

**Data Analyst’s Role:**
As a data analyst, you're tasked with:
- Analyzing customer reviews, campaign metrics, and engagement data.
- Providing actionable insights to optimize marketing strategies.
- Helping business improve ROI, boost engagement, and elevate customer satisfaction.

**Key Performance Indicators (KPIs):**
- **Conversion Rate** – % of visitors who purchase
- **Customer Engagement Rate** – Interactions like clicks, likes, comments
- **Average Order Value (AOV)** – Average spend per transaction
- **Customer Feedback Score** – Average product/service review rating

**Project Goals:**
- **Increase Conversion Rates:** Identify drop-off points in the funnel and recommend solutions.
- **Enhance Engagement:** Understand which content types drive higher interaction.
- **Improve Feedback Scores:** Extract and act on sentiment trends in reviews.


---

## 📁 Project Structure

```
DataAnalystPortfolioProject_PBI_SQL_Python_MarketingAnalytics-main/
│
├── Data/
│   ├── fact_customer_reviews_enrich.csv
│   └── MarketingAnalytics.bak              # SQL Server backup
│
├── SQL/
│   ├── dim_customers.sql
│   ├── dim_products.sql
│   ├── fact_customer_journey.sql
│   └── fact_customer_reviews.sql
|
├── Visualisation/
│   ├── Dashboard.pbix                      # Power BI file for data visualisation
│   └── Calendar DAX Script
│
├── customer_reviews_enrichment.py          # Python script for enriching review data
├── Final_Report.pptx                       # Final presentation of insights
└── README.md                               
```

---

## 🛠️ How to Run the Project

### 1. 📥 Restore SQL Database

Use **SQL Server Management Studio (SSMS)** or **Azure Data Studio** to restore the `MarketingAnalytics.bak` file:

- Open SSMS
- Right-click on `Databases` → `Restore Database`
- Select **Device** → Add the `.bak` file
- Restore the database

Run the scripts in `/SQL` to recreate or verify tables.

### 2. 🐍 Run Python Script

The script `customer_reviews_enrichment.py` enriches the reviews data.

#### Requirements

```bash
pip install pandas numpy
```

#### Run the Script

```bash
python customer_reviews_enrichment.py
```

Ensure the file `fact_customer_reviews_enrich.csv` is in the `Data/` folder.

### 3. 📊 Use with Power BI

- Import the CSV file and connect to the restored SQL database.
- Create reports for marketing performance, customer sentiment, and segmentation.

---

## 🧠 Insights Delivered

- Funnel analysis and optimization opportunities
- Customer sentiment trends and product feedback
- Demographic analysis to support targeting strategies
