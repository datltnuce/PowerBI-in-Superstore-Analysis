# 📊 Adventure Works Analysis  
Author: Dat Le Tien  
Date: 2025-02-15  
Tools Used: Power BI 

---

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset](#-dataset)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  

---

## 📌 Background & Overview  

### 📖 What is this project about? 

To monitor and optimize the manufacturing process by tracking production timelines, quality control, and inventory management, ensuring efficient operations and high-quality output.

### 👤 Who is this project for?  

✔️ Executive Team (CEO, CFO, COO)<br>
✔️ Sales & Marketing Team<br>
✔️ Operations & Supply Chain Team

### ❓Business Questions:  

✔️ What are the revenue trends across different regions and product categories?<br>
✔️ Which products contribute the most to profitability, and which underperform?<br>
✔️ Who are the most valuable customer segments, and how can we better serve them?<br>
✔️ What strategies can help expand into new markets while optimizing existing resources?

### 🎯Project Outcome:  

✔️ Clear insights into revenue, profitability, and operational efficiency.<br>
✔️ Identification of high-value products and customer segments for strategic focus.<br>
✔️ Improved resource allocation and cost optimization.<br>
✔️ Data-driven strategies for market expansion and competitive advantage.

---

## 📂 Dataset 
 
Orders: A table that stores transaction information.

People: A table that stores information about sales representatives in each region.

Returns: A table that records transactions that have been returned.

---

## 🧠 Design Thinking Process
### 1️⃣ Empathize
| 5W1H                                                          |                                           |
| ------------------------------------------------------------------ |--------------------------------------------- |
| Who will be viewing this Dashboard?                                | Sales manager, Marketing manager, Strategy manager<br> |
| If we had to choose only one key Stakeholder, who would it be?<br> | Sales manager |
| What problem does this Dashboard solve?                            | Overrall Business Performance, Market Analysis, Product Analysis.<br> |
| Describe the problem in one sentence                               | Help the Sales manager see overall business performance, therefore he can define good performing market and product.<br> |
| When and where will Stakeholders view this Dashboard?<br>          | In the meeting with the team in the office<br>Alone by themselves in the office at home or commuting |
| Why do stakeholders need this Dashboard?<br><br>                   | To see what is happening in the business<br>To see what did happen in the past<br>Verify their instinct and experienced assumption |
| How have stakeholders been achieving their goals so far?           | Finding potential market with high opportunity<br>Define which product should use to penetrate, to scale up<br>Balance between revenue and profit |


|Stakeholder Empathy Mapping                                                         |                                                          |
| ---------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pains                                                      | Does the growth trend happen to all the markets and all the products<br>What is the right go-to-market strategy for each country and each product                                                     |
| Thinking and feeling                                       | The sales manager thinks that the business performance is good, the company is doing well<br>They feel the win and want to go faster and bigger        |
| Seeing                                                    | The sales manager sees the growth trend in total revenue                                       |
| Saying and doing                                          | The sales manager wants to expand the business to various places because of the positive sign in market |
| Gains                                                     | Using data, the stakeholder can verify their assumptions in performance and find out details in each category. Avoid being bias and general, vague strategy                            |


| Fact table<br>                        | Dim table<br>                                                 |
| -------------------------------------- | -------------------------------------------------------------- |
| Orders | People, Return |

### 2️⃣ Define point of view

|                            | NORTHSTAR METRIC                         |
|----------------------------|--------------------------------------|
| **What VALUE you want to measure?** | Customer Lifetime Value                          |
| **WHEN the value DELIVERY SUCCESS?** | Successful delivery occurs when the customer is satisfied and continues to choose to shop at the store. |
| **Northstar Metric Name**  | Customer Lifetime Value                            |
| **WHY do you choose this metric?** | Customer Lifetime Value is a comprehensive and useful metric that helps businesses evaluate performance and develop sustainable growth strategies. |


Dimension Group
| Group 1 | Group 2  |
| ------- | -------- |
| Overview analysis | Return analysis |

Define Point of View
| View                     | Description                                                                                       | Why                                                                                                                     |
|--------------------------|---------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| View 1      | Provides a high-level overview of business performance, supporting strategic decision-making. | This dashboard offers a comprehensive view of the entire store's business operations, focusing on key financial metrics like revenue, profit, and profit margin. The information is presented at a high level, enabling managers to assess the overall performance of the business and make strategic decisions. The metrics are analyzed from various perspectives such as product categories, countries, cities, and individuals, helping managers understand the factors influencing business outcomes.    |
| View 2 | Focuses on a specific issue (return rates), supporting service quality improvement and operational efficiency.    | This dashboard concentrates on a specific issue: return rates. It's a crucial metric for evaluating customer satisfaction and operational efficiency. The data is presented in detail, broken down by time, customer segment, shipping method, and region, enabling relevant departments to identify the root causes of the issue and implement improvement measures. |
### 3️⃣ Ideate 
Brainstorming
| Idea Name               | Layer 0 Dimension: Total Metrics              | Layer 1 Dimension: Breakdown by 1 Dimension                                   | Layer 2 Dimension: Breakdown by 2 Dimensions                                           |
|-------------------------|-----------------------------------------------|--------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------|
| View 1       | Total sales<br>Total profit<br>Profit Ratio | Sales Trend for Total Sales and Profit<br>Sales by Category<br>Top 10 City by Sales<br>Sales by Country<br>Sales and Profit by Sub-Category<br>Top 5 Total Sales and Total Profit by Person | Sales Trend for Total Sales and Profit<br>Sales and Profit by Sub-Category<br>Top 5 Total Sales and Total Profit by Person          |
| View 2| Return Rate                  | Return Rate by Date<br>Return Rate by Segment<br>Return Rate by Ship Mode<br>Return Rate by Sub-Category<br>Return Rate by Region |                 |

### 4️⃣ Data modeling
![Image](https://github.com/user-attachments/assets/958aa84a-6923-41a2-b718-ed1f764229fe)

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ View 1: Overview Analysis
![Image](https://github.com/user-attachments/assets/e7385925-4d5e-4f3f-939b-bb6e4275f710)

### Insights:
- ***Total Sales**:* $32 billion with a ***profit ratio*** of 14.3%.
- ***Technology*** dominates with $25.85 billion in sales and a profit ratio of 15.44%.
- ***Office Supplies*** has the highest profit ratio (30.35%) despite lower sales.
- ***Furniture*** has a negative profit (-5.11%).

**Performance by City and Country**
- ***Mexico City*** leads with $0.99 billion in sales, followed by ***San Salvador*** with $0.86 billion.
- ***Top-performing countries**:* The U.S.

**Subcategories with negative profit**
- Significant losses: ***Chairs and Tables*** ***(same $382 million)***, profit ratio -41.56%.
### View 2: Return Analysis
![Image](https://github.com/user-attachments/assets/9c16374f-2745-4398-95a6-2306eb4e4f9d)

### Insights:
- The return rate is ***4.7%***, which is relatively high and could impact overall profit.
- ***Segment: Home Office*** has the highest return rate *(**35.38%**)*, followed by ***Corporate** (**33.21%**)* and ***Consumer** (**31.41%**).*
- ***Ship Mode: First Class*** and ***Same Day*** shipping methods have the highest return rates (6.38% and 6.47%, respectively).
- ***Region: North Asia,** **West*** regions have the highest return rates (13.83% and 11.73%, respectively) and ***Southeast Asia*** has the lowest return rate (3.63%).
- ***Subcategory:* *Copiers*** is the highest.

*b. Improve Rejection Rate:*
- Conduct quality checks at critical production stages to detect errors earlier.
- Increase automation in the production process to reduce human-related errors.

---
