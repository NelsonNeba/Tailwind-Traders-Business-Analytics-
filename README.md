
# Power BI Data Analyst Professional Certificate Capstone Project: Tailwind Traders Business Analytics

## Project Context
This project serves as the capstone for the **Microsoft Power BI Data Analyst Professional Certificate**, demonstrating mastery of key competencies including:
- **ETL Processes**: Data extraction, transformation, and loading from multiple sources
- **Data Modeling**: Creating efficient star schemas with proper relationships
- **DAX Programming**: Developing calculated columns, measures, and time intelligence
- **Visual Analytics**: Implementing best practices for effective data storytelling
- **Collaboration Features**: Configuring alerts, subscriptions, and mobile layouts

## Business Overview
Tailwind Traders is a multinational retail company requiring advanced analytics to optimize:
- Sales performance tracking
- Inventory management
- Regional profitability analysis
- Customer loyalty programs





## Project Components

### Part 1: Data Preparation & Modeling
- **Exercise 1**: Prepare Sales Excel Data
  - Calculated key financial metrics:
    - Gross Revenue (`=E2*G2`)
    - Total Tax (`=F2*G2`)
    - Net Revenue (`=H2-I2`)
  - Analyzed initial data trends

- **Exercise 2**: Configure Data Sources
  - Loaded and transformed 4 data sources:
    1. Sales data (Excel)
    2. Purchases data (Excel)
    3. Countries data (Excel)
    4. Currency Exchange data (Python script)
  - Optimized data types and validated data quality

- **Exercise 3**: Design Data Model
  - Created relationships between tables:
    - Countries ↔ Exchange Data (1:1)
    - Sales ↔ Countries (*:1)
    - Purchases ↔ Sales (1:1)
  - Developed calculated tables:
    - Calendar table (DAX)
    - Sales in USD table (DAX)

### Part 2: Aggregations & Reporting
- **Exercise 1**: Configure Aggregations (DAX)
  - Created key measures:
    - Yearly Profit Margin
    - Quarterly Profit
    - YTD Profit
    - Median Sales
  - Performance tested with Analyzer

- **Exercise 2**: Create Sales Report
  - Visualizations:
    - Loyalty Points by Country (Bar)
    - Quantity Sold by Product (Column)
    - Median Sales Distribution (Pie)
    - Median Sales Over Time (Line with forecast)
  - Interactive elements:
    - Country slicer
    - Card visuals for KPIs

- **Exercise 3**: Create Profit Report
  - Visualizations:
    - Net Revenue by Product (Bar)
    - Yearly Profit Margin by Country (Donut)
    - Yearly Profit Margin Over Time (Area)
  - Key metrics:
    - YTD Profit card
    - Net Revenue USD card
    - Gross Revenue USD KPI

### Part 3: Dashboard & Alerts
- **Exercise 6**: Executive Dashboard
  - Pinned key visuals from both reports
  - Configured mobile layout
  - Key findings:
    - UK has highest loyalty points (315)
    - Modular Sofa Set has highest net revenue ($928.36)
    - UAE has highest median sales ($680.79)

- **Exercise 7**: Alerts & Subscriptions
  - Created alert for Gross Revenue < $400
  - Set up subscriptions:
    - Sales Weekly Summary (Mondays 5AM)
    - Profit Weekly Summary (MWF 6AM)

## Technical Highlights
- **Data Transformation**: Cleaned and optimized multiple data sources
- **DAX Formulas**: Created time intelligence measures and currency conversions
- **Visual Storytelling**: Designed interactive reports with proper chart types
- **Automation**: Configured alerts and subscriptions for business monitoring

## Files Included
- `Tailwind Traders Sales.xlsx` - Source data
- `Countries.xlsx` - Source data
- `Purchases.xlsx` - Source data
- `Tailwind Traders Sales(Cleaned).xlsx` - Source data
- `Tailwind Traders Report.pbix` - Power BI report
- Python script for currency data (import pandas as pd from io import StringIO data = """Exchange ID;ExchangeRate;Exchange Currency 1;1;USD 2;0,75;GBP 3;0,85;EUR 4;3,67;AED 5;1 3;AUD"""
   df = pd.read_csv(StringIO(data), sep=';')
 
# Return the transformed dataframe
df
)

## How to Use
1. Open `Tailwind Traders Report.pbip` in Power BI Desktop
2. Refresh data connections if needed
3. Explore interactive reports and dashboard

## Key Insights
- Top performing product: Modular Sofa Set ($928.36 net revenue)
- Best sales region: UAE (highest median sales)
- Most loyal customers: UK (315 loyalty points)

## Recommendations  

Based on the analysis and insights generated, here are strategic recommendations for Tailwind Traders:

### 1. Product Strategy
- **Focus on High-Performing Products**  
  Prioritize inventory and marketing for the Modular Sofa Set (top net revenue generator) and similar high-margin products.
  
- **Review Low-Performing Items**  
  Investigate products with lowest net revenue (e.g., Floral Wallpaper at $9.60) for potential discontinuation or pricing strategy revision.

### 2. Customer Engagement
- **Loyalty Program Enhancement**  
  Leverage the UK's high loyalty points (315) to develop targeted retention campaigns. Consider expanding successful loyalty tactics to other regions.

- **Personalized Promotions**  
  Use sales rep performance data (e.g., Alice's 4 transactions) to identify best practices for sales team training.

### 3. Operational Improvements
- **Inventory Optimization**  
  Align stock levels with the quantity purchased patterns (average 2.8 units/transaction, max 6 units).

- **Warranty Strategy**  
  Adjust warranty offerings based on analysis (current average 18.88 months) to balance customer satisfaction and costs.

### 4. Geographic Expansion
- **UAE Market Focus**  
  Capitalize on UAE's highest median sales ($680.79) by increasing marketing investment and product availability in this region.

- **Currency Conversion Automation**  
  Implement real-time exchange rate updates beyond the current manual Python script solution.

### 5. Reporting Enhancements
- **Additional Time Intelligence**  
  Incorporate year-over-year comparison measures to track growth trends.

- **Customer Segmentation**  
  Add customer demographic data to enable more sophisticated RFM (Recency, Frequency, Monetary) analysis.

### 6. Technical Upgrades
- **Power BI Service Features**  
  Implement:
  - Data-driven alerts for inventory thresholds
  - Row-level security for regional managers
  - Paginated reports for operational data

- **Data Pipeline Improvement**  
  Migrate from Excel data sources to a cloud data warehouse for real-time data updates.

  ## Strategic Recommendations

### A. Commercial Opportunities
1. **Product Portfolio Optimization**
   - 🚀 *Action*: Create a product tiering system based on:
     - Top 20% by revenue (Modular Sofa Set, Power Drill Set)
     - Middle 60% 
     - Bottom 20% (Floral Wallpaper)
   - 📈 *Expected Impact*: 18-22% increase in inventory turnover

2. **Geographic Expansion Strategy**
   - 🌍 *Priority Markets*: UAE (680.79 median sales) and UK (315 loyalty points)
   - 💡 *Tactics*: Localized marketing campaigns and distribution partnerships

### B. Operational Improvements
1. **Dynamic Pricing Model**
   - ⚙️ *Implementation*: DAX-powered price elasticity analysis
   - 🕒 *Timeline*: Phase 1 in 3 months

2. **Sales Team Incentivization**
   - 📊 *Based On*: Alice's high-performance pattern (4 transactions)
   - 🎯 *Metrics*: Customer retention rate + basket size

### C. Technical Enhancements
1. **Data Infrastructure**
   | Current | Recommended | Benefit |
   |---------|-------------|---------|
   | Excel Files | Azure SQL DB | Real-time updates |
   | Static Exchange Rates | Power Automate Flow | Automated refreshes |

2. **Advanced Analytics**
   - Predictive inventory forecasting
   - Customer lifetime value modeling
   - AI-powered product recommendations



## Implementation Roadmap  

| Priority | Recommendation | Estimated Impact | Timeline |
|----------|----------------|------------------|----------|
| High | Focus on top-performing products | ↑ Revenue 15-20% | 1-2 months |
| High | UAE market expansion | ↑ Market share 5-8% | 3-6 months |
| Medium | Loyalty program enhancements | ↑ Retention 10% | 2-4 months |
| Medium | Inventory optimization | ↓ Carrying costs 12% | 1-3 months |
| Low | Technical upgrades | ↑ Efficiency 30% | 6-12 months |


## Certification Competencies Demonstrated

| Skill Area | Project Artifacts | Microsoft Exam Alignment |
|------------|-------------------|--------------------------|
| Data Preparation | Sales/Purchases data transformation | PL-300: Prepare the Data |
| Data Modeling | Star schema with 5 tables | PL-300: Model the Data |
| Visualization | 8 interactive reports | PL-300: Visualize the Data |
| Deployment | Dashboard subscriptions | PL-300: Deploy Solutions |