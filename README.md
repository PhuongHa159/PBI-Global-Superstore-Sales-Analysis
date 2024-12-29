# PBI-Global-Superstore-Sales-Analysis
## I. Introduction
This project utilizes the Superstore company's sales data to analyze the company's business performance in order to develop market expansion strategies and make strategic product selection decisions. The business analysis by product and market will highlight potential products and markets. This Power BI project provides a visual perspective, supporting data-driven decision-making for the development of effective strategies.

## II. Dataset
Dataset : "PBI-Global Superstore Sales Analysis-DATASET" (attached above)
The dataset contains global sales information for a company called Superstore, and includes three tables:
- **Orders:** A table that stores transaction information.
- **People:** A table that holds information about salespeople in different regions.
- **Returns:** A table that records transactions that were returned.

## III. Design Thinking Steps

### Stage 1: Empathize
**5W1H**
| 5W1H |  |
| --- | --- |
| Who will view this dashboard? | The company's product managers and senior managers. |
| If only one key stakeholder is to be selected, who will it be? | Senior managers. |
| What issue does this dashboard address? | It provides a snapshot of the company's business situation, helping to develop market expansion strategies and decide on strategic products. |
| Use one sentence to describe the issue: | Defining strategic products and identifying potential markets for growth. |
| When and where will stakeholders view this dashboard? | Product managers will view it when they need to review the products launched on the market and when they want to create a new product.<br>Senior managers will view it when they need to assess the company's business performance, make decisions on market expansion strategies, and select strategic products in discussion meetings. |
| Why do stakeholders need this dashboard? | To assess the overall business situation in different regions<br>To identify strategic products for the company<br>To identify potential areas for market expansion. |
| How have stakeholders achieved their goals? | Product managers: By understanding the sales, returns, and growth rates in various markets to select potential markets and identify areas that need improvement<br>Senior managers: By assessing sales, returns, and growth rates by product category to select strategic products. |

**EMPATHY MAP and STAKEHOLDER JOURNEY**

| EMPATHY MAP |  |
| --- | --- |
| Thinking and feeling<br>What does the stakeholder think and feel? | The company is running well, but I want it to grow even more, with the goal of achieving this year's revenue target first. |
| Seeing<br>What does the stakeholder see? | The company is performing well on a global scale<br>This year's revenue target is set higher than last year. |
| Saying and doing<br>What does the stakeholder say? | "I believe expanding into new markets can help the company achieve its revenue target."<br>"To increase revenue, I should also review the current markets to see if there's anything that needs improvement." |
| Pains<br>What are the biggest problems and challenges? | Which markets are potential for expansion?<br>Do we need to improve the current markets?<br>Which products should we focus on for new or existing markets? |
| Gains<br>What are the opportunities and benefits? | Identifying potential products and growing markets => Adjusting strategy to focus on high-profit opportunities => Increasing revenue and effectively expanding market share<br>Determining revenue and market trends will help predict risks and adjust strategy in a timely manner. |

| STAKEHOLDER JOURNEY |  |
| --- | --- |
| Step 1: | Based on the goal of increasing revenue, the senior manager will have two solution approaches:<br>Improve current markets<br>Develop new markets |
| Step 2: | To make an informed decision, the senior manager provides the DA team with historical data on sales/returns/salespersons, and the order team analyzes and visualizes it. |
| Step 3: | After obtaining the draft dashboard, the senior manager checks if the dashboard answers the questions and solves the issues.<br>Are there any additional ideas that need to be explored?<br>Does anything need improvement in the dashboard? |
| Step 4: | Use the finalized dashboard to assess the situation, make decisions, and develop strategies.<br>This outline highlights the steps the senior manager takes in utilizing data and a dashboard for decision-making and strategy development. |

### Stage 2: Define POV
**Northstar Metric**
| NORTHSTAR  |  |
| --- | --- |
| What VALUE you want to measure? | The profit of each product and each market |
| WHEN the value DELIVERY SUCCESS? | When the product is successfully delivered and not returned |
| Northstar Metric Name | Profit |
| WHY do you choose this metric? | Profit reflects the company's business situation. Products and markets with higher profit are more potential for development |

**Define Point of View**

| Dimension Data Group |   |    | 
| --- | --- |--- |
| Group 1  | Business performance year by year  | Product<br>Market<br>Customer Info |
| Group 2 | Product | Category<br>Sub Category |
| Group 3 | Market | State<br>Market<br>Region |
| Group 4 | Customer Info | Customer ID<br>Customer name<br>Segment |

| View | Description |  Why | 
| --- | --- |--- |
| Product | Product Data | Provides insights into product revenue |
| Market |  Market Data | Provides insights into market revenue |
| TBusiness Performance | Overall data on revenue and profit by year | Provides insights into the company's business performance |

### Stage 3: Ideate

**BRAINSTORMING**
| Overview layer | |
| --- | --- |
|**Metric 1** | Revenue |
|**Metric 2** | Profit |
|**Metric 3** | Profit Margin |
|**Metric 4** | Return Rate |

| **Idea Name** | **Layer 0 dimension** | **Layer 1 dimension** | **Layer 2 dimension** |
| --- | --- | --- | --- |
| View 1: OVERVIEW | 1. Total Revenue<br>2. Total Profit | Total revenue and Total cost by category and market |   |   |
| View 2: Product | 1. Total Revenue<br>2. Total Profit | 1. Revenue by product category<br>2. Profit  by product category<br>3. Product Classification:- High vol, High profit- High vol, Low profit- Low vol, High profit- Low vol, Low profit<br>4. Profit margin by product category<br>5. Return rate by product category| 1. Revenue, profit by category, by year |  |
| View 3: Market | 1. Total Revenue<br>2. Total Profit3. Total Number of Customer | 1. Revenue by market<br>2. Profit by market<br>3. Profit Margin by market<br>4. Customer number by market<br>5. Return Rate by market | 1. Revenue, profit by market, by category |  |

**STRUCTURE IDEA**

| Scorecard ||
| --- | --- |
| Metric 1 | Revenue|
|**Metric 2 | Number of customers|
|Metric 3 | Profit|
|Metric 4 | Profit Margin|

| Idea Name | Very Important Information | Important Information | Detailed Information |
| --- | --- | --- | --- |
| View 1 | 1. Total revenue<br>2. Total number of orders | 1. Revenue and profit margin<br>2. Return rate| 1. Total revenue by customer, category, and market<br>2.Total number of orders over the years<br>3. Revenue and profit margin by category and market |
| View 2 | 1. Revenue by product category<br>2. Profit by product category <br>3.Product Classification<br>4. Profit margin by product category<br>5. Return rate by product category | 1. Total Revenue<br>2. Total Profit| 1. Revenue, profit by category, by year |
| View 3 | 1. Revenue by market<br>2. Profit by <br>. Profit Margin by market<br>4. Customer number by market<br>5. Return Rate by market | 1. Total Revenue<br>2. Total Profit<br>3. Total Number of Customer | 1. Revenue, profit by market, by category<br>2. Market details |

**Next, I proceeded with **Step 4 - Prototype and Review** multiple times and achieved the final result, which will be presented in the following section as a dashboard.**

## III. Dashboard

**Model View**

<img width="506" alt="model" src="https://github.com/user-attachments/assets/744fa171-d648-4c20-a922-6d59c79508e6" />

**1. Overview**

<img width="574" alt="overview" src="https://github.com/user-attachments/assets/186cab23-3af3-4dbb-b24d-4eed7803103b" />

**2. Product**

<img width="574" alt="Product" src="https://github.com/user-attachments/assets/68917d7b-f108-491c-916c-39b7fe2ada3a" />

**3. Market**

<img width="574" alt="market" src="https://github.com/user-attachments/assets/e9f9d3ca-917d-466e-95f4-688d2f7d1879" />

## IV. Insight

**OVERVIEW**
- Sales and Profit have shown consistent growth over the years. By 2014, both metrics had doubled compared to 2011. However, the return on sales (ROS) experienced a downward trend between 2013 and 2014, decreasing by 0.58%.
- The Consumer segment accounts for the largest share of revenue, reaching $6.51M (approximately 50%).
- The refund rate has been declining over the years, dropping from 6.1% in 2011 to 5.72% in 2014, a reduction of 0.38%.

**PRODUCT**
- **Home Supplies** accounts for the largest proportion of product volume, at 61.01%.
- **Paper** has the highest ROS, reaching 26.29%, but its order volume is only average, with 3.8K orders over 4 years.
- **Tables** are currently unprofitable, with a total loss of $31K over 4 years.
- **Canon ImageCLASS2000** is the most profitable product during 2013–2014, generating $9.0K in profit. However, it also has a high return volume, amounting to $6.7K.

**MARKET**
- **Canada** has the highest ROS (26.62%), but its revenue and order volume remain unimpressive, with revenue at $66.93K and only 833 orders.
- **APAC** is the most profitable market for the company, showing particularly strong growth between 2012 and 2014. Among APAC countries, **India** contributes the most, accounting for nearly one-third of the region's total profit at $125,492. Total profit from APAC reaches $389,324, approximately 29% of the company's global profit ($1,349,557).

## V. Recommendation
- **Focus on increasing overall profitability:**
    - Optimize the supply chain to reduce operational costs.
    - Conduct cost-benefit analyses to identify and eliminate products or services that provide low value.
- **Develop sales and marketing strategies for Paper products:**
    - Strengthen marketing campaigns targeting key distribution channels and primary customers.
    - Launch promotional programs or discounts to stimulate demand.
    - Introduce bundled packages that combine Paper with related items to increase order value.
- **Reduce costs and optimize Tables products:**
    - Reassess the product pricing strategy.
    - Seek alternative suppliers offering lower-cost materials while maintaining quality.
- **Improve the Canon ImageCLASS2000 product to minimize return risks:**
    - Collect customer feedback to identify the main causes of returns.
    - Enhance product quality based on feedback or provide more detailed usage instructions.
    - Offer warranty policies or quick technical support to reduce return rates.
- **Develop strategies to unlock the potential of the Canadian market:**
    - Invest in promotional campaigns focused on raising brand awareness in Canada.
    - Partner with local distributors to increase customer reach.
    - Establish warehousing or distribution centers in Canada to lower shipping costs.
- **Continue strong investment in the APAC market, especially in India:**
    - Expand distribution networks in untapped areas of India.
    - Strengthen strategic partnerships with local retailers.
