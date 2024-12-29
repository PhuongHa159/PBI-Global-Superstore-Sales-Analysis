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
| Ai sẽ là người xem Dashboard này? | 1. Các nhà quản lý sản phẩm của công ty 
2. Các Senior Manager |
| Nếu chỉ chọn 1 key Stakeholder thì đó sẽ là ai? | Các nhà quản lý cấp cao |
| Dashboard này giải quyết vấn đề gì? | Giúp phác họa bức tranh về tình hình kinh doanh của công ty để đưa ra các chiến lược mở rộng thị trường và quyết định lựa chọn sản phầm chiến lược |
| Dùng 1 câu để mô tả vấn đề | Định hướng sản phẩm chiến lược và thị trường tiềm năng để phát triển |
| Stakeholder sẽ xem Dashboard này khi nào và ở đâu? | 1. Các nhà quản lý sản phẩm sẽ xem dashboard khi họ cần review lại các sản phẩm đã tung ra thị trường và khi họ muốn tạo ra một sản phẩm mới 
2. Các Senior Manager  sẽ xem dashboard khi họ cần đánh giá các hiệu quả kinh doanh của công ty,đưa ra các quyết định về chiến lược mở rộng thị trường và quyết định sản phẩm chiến lược trong các buổi họp thảo luận |
| Tại sao các stakeholder cần Dasboard này? | 1. Đánh giá tổng thể tình hình kinh doanh của công ty tại các khu vực 2. Tìm ra sản phẩm chiến lược cho công ty 
3. Xác định các khu vực tiềm năng để mở rộng thị trường |
| Stakeholder đã làm như thế nào để đạt được mục tiêu | 1. Nắm được tình hình bán hàng, trả hàng, tốc độ tăng trưởng của các thị trường --> Chọn được thị trường tiềm năng --> Biết được thị trường nào cần cải thiện (Từ đó có kế hoạch tìm hiểu nguyên nhân và đưa ra giải pháp cải thiện) 
2. Nắm được tình hình bán hàng, trả hàng, tốc độ tăng trưởng theo danh mục sản phẩm --> Chọn được sản phẩm chiến lược |

**EMPATHY MAP and STAKEHOLDER JOURNEY**

| Thinking and feelingWhat does the stakeholder think and feel? |  |SeeingWhat does the stakeholder see? |  | Saying and doingWhat does the stakeholder say?|  |
| --- | --- | --- | --- | --- | --- |
| - Công ty đang vận hành tốt, mình muốn công ty phát triển hơn nữa, trước mắt là đạt mục tiêu doanh thu năm nay. |  | - Công ty đang vận hành tốt trên quy mô toàn cầu.- Mục tiêu doanh thu của năm nay đề ra cao hơn năm trước. |  | - Mình tin rằng việc mở rộng thị trường mới có thể giúp công ty đạt mục tiêu doanh thu.- Để tăng doanh thu, mình cũng nên xem lại tình hình ở các thị trường hiện tại xem có gì cần cải thiện không? |  |
| Pains What are the biggest problems and challenges? |  | Gains What are the opportunities and benefits? |  |  |  |
| - Đâu là thị trường tiềm năng để mở rộng?- Có cần cải thiện các thị trường hiện tại không?- Đâu là sản phẩm tiềm năng để tập trung cho thị trường mới/cũ? |  | Nhận biết được các sản phẩm nào có tiềm năng, thị trường nào đang phát triển => điều chỉnh chiến lược tập trung vào các cơ hội sinh lời cao => tăng doanh thu và mở rộng thị phần hiệu quả
Xác định được doanh thu và xu hướng thị trường sẽ giúp dự đoán trước được những rủi ro và điều chỉnh chiến lược kịp thời |  |  |  |
|  |  |  |  | **STAKEHOLDER JOURNEY** |  |
| **Step 1:** |  | **Step 2:** |  | **Step 3:** | **Step 4:** |
| Dựa vào mục tiêu tăng doanh thu, senior manager sẽ có 2 hướng giải pháp:- Cải thiện thị trường hiện tại- Phát triển thị trường mới |  | Để có được cơ sở đưa ra lựa chọn, senior manager cung cấp cho team DA các dữ liệu bán hàng/hoàn hàng/sales person trong lịch sử và order team DA phân tích và trực quan hóa |  | Sau khi đã có được bản draft dashboard, senior manager check xem DB đã trả lời được câu hỏi, giải quyết được vấn đề chưa? Có thêm ý tưởng nào cần đào sâu không? Có cần cải thiện gì ở DB không? | Sử dụng bản DB hoàn thiện để đánh giá tình hình, đưa ra quyết định và chiến lược |

### Stage 2: Define POV

| NORTHSTAR  |  |
| --- | --- |
| What VALUE you want to measure? | Lợi nhuận của từng sản phẩm và từng thị trường |
| WHEN the value DELIVERY SUCCESS? | Khi sản phẩm được giao thành công và không bị trả lại |
| Northstar Metric Name | Profit |
| WHY do you choose this metric? | Lợi nhuận thể hiện tình hình kinh doanh của công ty. Sản phẩm và thị trường mang lợi nhuận càng cao thì càng tiềm năng để phát triển. |

| Define Point of View |  |  |  |  |
| --- | --- | --- | --- | --- |
| Dimension Data Group | Group 1 | Group 2 | Group 3 | Group 4 |
|  | Tình hình kinh doanh qua từng năm | Product | Market | Customer Info |
|  | Sales, profit, order, return rate | Category, Sub Category | State, Market, Region | Customer ID, Customer name, Segment |
|  |  |  |  |  |
| View | Description |  | Why |  |
| Product | Dữ liệu về sản phẩm |  | Cung cấp góc nhìn về doanh thu sản phẩm |  |
|  |  |  |  |  |
| Tình hình kinh doanh | Dữ liệu tổng quát về doanh thu, lợi nhuận theo từng năm |  | Cung cấp góc nhìn về tình hình kinh doanh của công ty |  |

### Stage 3: Ideate
**BRAINSTORMING**
                  | BRAINSTORMING               |
| --- | --- | --- | --- | --- |
| Overview layer | **Metric 1** | **Metric 2** | **Metric 3** | **Metric 4** |
|  | Revenue | Profit | Profit Margin | YoY Growth Rate |
|  | **Metric 5** | **Metric 6** | **Metric 7** | **Metric 8** |
|  | Number of customers | Return Rate |  |  |
| **Idea Name** | **Layer 0 dimension: chỉ số tổng** | **Layer 1 dimension: chỉ số được breakdown theo 1 chiều** | **Layer 2 dimension: chỉ số được breakdown theo 2 chiều** | **Có điều gì quan trọng mình bỏ lỡ không?** |
| View 1: OVERVIEW | 1. Total Revenue2. Total Profit | Total revenue and Total cost by category and market |   |   |
| View 2: Product | 1. Total Revenue2. Total Profit | 1. Revenue by product category2. Profit  by product category3. Product Classification:- High vol, High profit- High vol, Low profit- Low vol, High profit- Low vol, Low profit4. Profit margin by product category5. Return rate by product category6. YoY Growth Rate of Revenue by product category | 1. Revenue, profit by category, by year |  |
| View 3: Market | 1. Total Revenue2. Total Profit3. Total Number of Customer | 1. Revenue by market2. Profit by market3. Profit Margin by market4. Customer number by market5. Return Rate by market6. YoY Growth Rate of Revenue by market | 1. Revenue, profit by market, by category |  |

**STRUCTURE IDEA**

| STRUCTURE IDEA |
| --- | --- | --- | --- | --- | --- | --- | --- |
|  | **Metric 1** | **Metric 2** | **Metric 3** | **Metric 4** | **Metric 5** | **Metric 6** |  |
| **Scorecard** | **Revenue** | **Number of customers** | **Profit** | **Profit Margin** |  |  |  |
| **Idea Name** | **Thông tin rất quan trọng** |  |  | **Thông tin quan trọng** |  |  | **Thông tin chi tiết** |
| View 1 | 1. Revenue by market2. Profit by market3. Profit Margin by market4. Customer number by market5. Return Rate by market6. YoY Growth Rate of Revenue by market |  |  | 1. Total Revenue2. Total Profit3. Total Number of Customer |  |  | 1. Revenue, profit by market, by category2. Market details |

**#### Next, I proceeded with **Step 4 - Prototype and Review** multiple times and achieved the final result, which will be presented in the following section as a dashboard.**

## III. Dashboard

Model View

<img width="506" alt="model" src="https://github.com/user-attachments/assets/744fa171-d648-4c20-a922-6d59c79508e6" />

1. Overview

<img width="574" alt="overview" src="https://github.com/user-attachments/assets/186cab23-3af3-4dbb-b24d-4eed7803103b" />

2. Product

<img width="574" alt="Product" src="https://github.com/user-attachments/assets/68917d7b-f108-491c-916c-39b7fe2ada3a" />

3. Market

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
- **1. Focus on increasing overall profitability:**
    - Optimize the supply chain to reduce operational costs.
    - Conduct cost-benefit analyses to identify and eliminate products or services that provide low value.
- **2. Develop sales and marketing strategies for Paper products:**
    - Strengthen marketing campaigns targeting key distribution channels and primary customers.
    - Launch promotional programs or discounts to stimulate demand.
    - Introduce bundled packages that combine Paper with related items to increase order value.
- **3. Reduce costs and optimize Tables products:**
    - Reassess the product pricing strategy.
    - Seek alternative suppliers offering lower-cost materials while maintaining quality.
- **4. Improve the Canon ImageCLASS2000 product to minimize return risks:**
    - Collect customer feedback to identify the main causes of returns.
    - Enhance product quality based on feedback or provide more detailed usage instructions.
    - Offer warranty policies or quick technical support to reduce return rates.
- **5. Develop strategies to unlock the potential of the Canadian market:**
    - Invest in promotional campaigns focused on raising brand awareness in Canada.
    - Partner with local distributors to increase customer reach.
    - Establish warehousing or distribution centers in Canada to lower shipping costs.
- **6. Continue strong investment in the APAC market, especially in India:**
    - Expand distribution networks in untapped areas of India.
    - Strengthen strategic partnerships with local retailers.
