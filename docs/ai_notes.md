###### \##AI Documentation

###### 

###### \## Prompt 1:

I have the following datasets: Superstore Sales, Telco Churn, Twitter Sentiment, COVID-19.  

Suggest 5 high-value KPIs and questions to answer for each.



###### \## AI Response:

📊 1. **Superstore Sales Dataset**

**🔹 KPIs**



🔹**Total Sales, Profit \& Profit Margin (%)**



How much revenue and profit are we generating, and which products/regions drive margins?



🔹**Sales Growth Rate (MoM or YoY)**



Are sales improving over time, or are we declining in specific months/years?



🔹**Top \& Bottom Performing Categories/Sub-Categories**



Which product lines bring maximum sales/profit? Which ones drag performance?



🔹**Customer Lifetime Value (CLV) using RFM (Recency, Frequency, Monetary)**



Which customers are most valuable to retain?



🔹**Average Shipping Delay (Order Date → Ship Date)**



Is our shipping efficient? Does delay affect customer satisfaction or profitability?



🔹 **Questions to Answer**



* Which region contributes the most to profit margin?
* Are discounts helping increase sales or eroding profits?
* Which customers/products generate the highest lifetime value?
* How does shipping delay vary across regions or product categories?
* What seasonal patterns affect sales performance?



📞 2. **Telco Churn Dataset**

**🔹 KPIs**



🔹**Churn Rate (%)**



What percentage of customers leave the service each month?



🔹**Customer Retention Rate (%)**



How effective are we at keeping existing customers?



🔹**Average Revenue Per User (ARPU)**



How much revenue does each customer generate on average?



🔹**Tenure vs. Churn Relationship**



Do long-term customers churn less?



🔹**Churn by Customer Segment (Contract Type, Internet Service, Payment Method)**



Which groups of customers are more likely to churn?



🔹 **Questions to Answer**



* What are the top 3 drivers of customer churn (e.g., contract type, monthly charges, service issues)?
* Do customers on month-to-month contracts churn more than yearly contract customers?
* How does churn differ between fiber optic and DSL customers?
* Are high-paying customers more loyal, or do they churn faster?
* Which retention offers could reduce churn in high-risk groups?



###### \## Prompt 2:

Here’s my dataset’s missing value summary. Suggest a cleaning approach with Pandas code.



###### \## AI Response:

\- Drop duplicate rows with `df.drop\_duplicates()`.  

\- Convert date columns using `pd.to\_datetime()`.  

\- Fill missing values in numerical columns with `df\['col'].fillna(df\['col'].median())`.  

\- Create new calculated fields: `Profit Margin`, `Sales per Quantity`, `Order Month`.



###### \## Prompt 3:

What are 3 more calculated fields useful for sales analysis and their Pandas code?



###### \## AI Response:

🔹 **1. Profit Margin (%)**



👉 Helps measure profitability relative to sales.



df\['Profit Margin %'] = (df\['Profit'] / df\['Sales']) \* 100



**🔹 2. Sales per Quantity (Unit Price)**



👉 Useful for checking average selling price per unit.



df\['Sales per Quantity'] = df\['Sales'] / df\['Quantity']



**🔹 3. Shipping Delay (Days)**



👉 Measures efficiency of shipping process.



df\['Shipping Delay'] = (df\['Ship Date'] - df\['Order Date']).dt.days

