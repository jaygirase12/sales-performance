**##KPI**



**## Prompt 1**:“I have Superstore sales data with Sales, Profit, Quantity, Discount, and Dates. Suggest 5 KPIs a business manager would care about and DAX measures to calculate them in Power BI.”



**##AI Response:**

**📊 KPI 1: Total Sales**



**How much revenue is being generated.**



**Total Sales = SUM(Superstore\[Sales])**



**📊 KPI 2: Total Profit**



**How much money remains after subtracting costs.**



**Total Profit = SUM(Superstore\[Profit])**



**📊 KPI 3: Profit Margin (%)**



**How efficient sales are at generating profit.**



**Profit Margin % =** 

**DIVIDE(**

    **\[Total Profit],**

    **\[Total Sales],**

    **0**

**)**



**📊 KPI 4: Sales Growth (Month-over-Month)**



**Tracks whether sales are increasing compared to last month.**



**Sales Growth MoM =** 

**DIVIDE(**

    **\[Total Sales] - CALCULATE(\[Total Sales], DATEADD(Superstore\[Order Date], -1, MONTH)),**

    **CALCULATE(\[Total Sales], DATEADD(Superstore\[Order Date], -1, MONTH))**

**)**



**📊 KPI 5: Average Discount**



**Shows how much discount is being offered on average.**



**Average Discount = AVERAGE(Superstore\[Discount])**

