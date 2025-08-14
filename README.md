# eCommerce Analysis sales of SuperStore using PowerBI
Sử dụng PowerBI để trình bày cho các senior manager về tình hình kinh doanh của công ty để đưa ra chiến lược mở rộng thị trường và quyết định lựa chọn sản phẩm chiến lược

---
 
Author: Nguyễn Hải Long  
Date: 2025-03   
Tools Used: Power BI  
---

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
5. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)

---

## 📌 Background & Overview  

### Objective:
### 📖 What is this project about? 
 
- Provide a brief introduction to the project. Define the problem statement/ business question that this project will show and why it is important.
- Write in bullet point format

 _Example:_

 This project analyzes sales trends and inventory control using SQL and Power BI. The objective is  
✔️ Identify high-demand products and sales trends.  
✔️ Optimize inventory levels to prevent overstocking or stockouts.  
✔️ Provide actionable insights through Power BI dashboards.  

### 👤 Who is this project for?  

Mention who might benefit from this project 

 _Example:_

✔️ Data analysts & business analysts  
✔️ Supply chain managers & inventory controllers  
✔️ Decision-makers & stakeholders  

---

## 📂 Dataset Description & Data Structure  

### 📌 Data Source  
- Source: Company database  
- Size: The dataset has 3 tables: Orders, People, Returns. Orders (20 columns, 51293 rows); People (2 columns, 15 rows); Returns (2 columns, 1174 rows).    
- Format: .csv  

### 📊 Data Structure & Relationships  

#### 1️⃣ Tables Used:  
Using 3 tables in .csv format

#### 2️⃣ Table Schema & Data Snapshot  

#### Table schema  

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_1_dataset.png)  

<details>
 <summary>Table 1: "Orders" table:</summary>

 | Column Name | Data Type | Description |  
 |-------------|----------|-------------|  
 | Order ID | TEXT | ID of orders |
 | Order Date | DATE | Date for orders |  
 | Ship Date | DATE | Delivery date |  
 | Ship Mode | TEXT | Delivery mode |
 | Customer ID | TEXT | ID of customers |
 | Customer Name | TEXT | Name of customers |
 | Segment | TEXT | Customers segmentation |
 | City | TEXT | Order location (city) |
 | State | TEXT | Order location (state) |
 | Country | TEXT | Order location (country) |
 | Postal Code | WHOLE NUMBER | Postal code |
 | Market | TEXT |
 | Region | TEXT |
 | Product ID | TEXT | ID of products |
 | Category | TEXT | Products segmentation |
 | Sub-Category | TEXT | Products sub-segmentation |
 | Product Name | TEXT | Name of products |
 | Sales | DECIMAL NUMBER | Products sales |
 | Quantity | WHOLE NUMBER | Products selling number |
 | Profit | DECIMAL NUMBER | Products profit |

</details>

<details>
 <summary>Table 2: "People" table:</summary>

 | Column Name | Data Type | Description |  
 |-------------|----------|-------------|  
 | Person | TEXT | Manager name | 
 | Region | TEXT | Management location |

</details>

<details>
 <summary>Table 3: "Returns" table:</summary>

 | Column Name | Data Type | Description |  
 |-------------|----------|-------------|  
 | Order ID | TEXT | ID of returned orders | 
 | Returned | TEXT | Returned confirmation |

</details>

#### 3️⃣ Data Relationships:  

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/table_schema.png)

- The connection between Returns.csv and Orders.csv is one-to-many with column "Order ID".
- The connection between People.csv and Orders. csv is one-to-many with column "Region".    

---

## 🧠 Design Thinking Process  

Explain the step-by-step approach taken to solve the problem.  

👉🏻 Insert a screenshot of the Design Thinking steps (Screenshot your Excel design thinking tables for better presentation).  

1️⃣ Empathize  

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_1_5w1h_1.png)

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_1_5w1h_2.png)

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_1_empathy_map.png)

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_1_stakeholde_need.png)

2️⃣ Define point of view  
3️⃣ Ideate  
4️⃣ Prototype and review  

---

## ⚒️ Main Process

1️⃣ Data Cleaning & Preprocessing 
2️⃣ Exploratory Data Analysis (EDA)  
3️⃣ SQL/ Python Analysis 

- In each step, show your Code

- Include query/ code execution screenshots or result samples

- Explain its purpose and its findings


4️⃣ Power BI Visualization  (applicable for PBI Projects)

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Dashboard 1 Preview  
👉🏻 Insert Power BI dashboard screenshots here  

📌 Analysis 1:  
- Observation: _Describe trends, key metrics, and patterns. Any insights from those observation_  
- Recommendation: _Suggest actions based on insights._  

#### 2️⃣ Dashboard 2 Preview  
👉🏻 Insert Power BI dashboard screenshots here

📌 Analysis 2:   
- Observation: _Describe trends, key metrics, and patterns. Any insights from those observation_  
- Recommendation: _Suggest actions based on insights._  

#### 3️⃣ Dashboard 3 Preview  
👉🏻 Insert Power BI dashboard screenshots here  

📌 Analysis 3:  
- Observation: _Describe trends, key metrics, and patterns. Any insights from those observation_  
- Recommendation: _Suggest actions based on insights._  

---

## 🔎 Final Conclusion & Recommendations  

👉🏻 Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following:  

📌 Key Takeaways:  
✔️ Recommendation 1  
✔️ Recommendation 2  
✔️ Recommendation 3
