# Sales Performance Analysis with AI Insights

## 📌 Overview
This project analyzes retail sales data from the Superstore dataset.  
The goal is to identify key performance indicators (KPIs), clean the dataset, and prepare it for analysis.  
AI (ChatGPT) was integrated to suggest KPIs and cleaning strategies.

## 📊 Dataset
- Source: [Superstore Dataset – Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
- Raw file: `/data/Superstore.csv`

## 🧠 AI Contribution
- Suggested KPIs for sales analysis
- Recommended cleaning strategies for missing values and duplicates
  - AI suggested:
  - Feature engineering ideas (Profit Margin, Sale per quantity, Shipping Delay)
  - Handling missing values with median imputation

## 📂 Project Structure
/data → raw & cleaned datasets
/notebooks → Jupyter notebooks
/reports → PDFs, dashboard screenshots
/docs → AI documentation

## ⚙️ Project Workflow
1. **Data Cleaning & Preprocessing**
   - Removed duplicates & missing values
   - Converted dates to datetime
   - Engineered features (Profit Margin, Order Month, Order Year)

2. **Exploratory Data Analysis (EDA)**
   - Sales by category, region, and customer segment
   - Time series trends for monthly and yearly sales
   - Profitability analysis

3. **Dashboard (Power BI)**
   - KPIs: Total Sales, Profit, Profit Margin %, Sales Growth
   - Visuals: Category-wise sales, Regional breakdown, Top 10 customers, Monthly trends

4. **AI-Assisted Insights**
   - Suggested KPIs via ChatGPT
   - Summarized insights into business-friendly language
   - Generated sample stakeholder Q&A

## Key Findings

📌 Technology leads in sales (~$0.8M), while Furniture and Office Supplies contribute slightly less; however, profit margins remain modest across all categories.

📌 East and West regions dominate sales, whereas Central shows weaker performance, highlighting room for regional growth.

📌 High discounts (avg. 15.6%) are squeezing profit margins (12.5%), showing that aggressive discounting directly reduces profitability.

📌 Top 10 customers contribute a large share of revenue, creating dependency risk — diversification of customer base is needed.

📌 Monthly trend shows spikes but inconsistent growth, indicating seasonality and the need for smoother demand planning.

## 📊 Dashboard
- 📄 File: `reports/sales_dashboard.pbix`
- 📷 Screenshots: `reports/visuals/`
