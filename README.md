# eCommerce Analysis sales of SuperStore using PowerBI  

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
 
- Real Canadian Superstore is a chain of supermarkets owned by Canadian food retailing giant Loblaw Companies. Its name is often shortened to Superstore.  
- The Senior Manager needs a clear view of the company’s overall business performance in order to define market expansion strategies and make informed decisions on strategic product selection.  
- Design a dashboard that enables stakeholders to address these needs effectively.  
- This project analyzes sales, profit trends using Power BI. The objective is:  
✔️ Gain an overall view of the company’s business performance from 2011 to 2014.  
✔️ Analyze Profit, Revenue, and Sales at both product and category product to identify strategic products.  
✔️ Explore regions and country-level markets to support decision-making on market expansion opportunities.  

### 👤 Who is this project for?  

✔️ Data analysts & business analysts.  
✔️ Supply chain managers.   
✔️ Decision-makers & stakeholders.  

---

## 📂 Dataset Description & Data Structure  

### 📌 Data Source  
- Source: Company database  
- Size: The dataset has 3 tables: Orders, People, Returns. Orders (20 columns, 51293 rows); People (2 columns, 15 rows); Returns (2 columns, 1174 rows).    
- Format: .csv  

### 📊 Data Structure & Relationships  

#### 1️⃣ Tables Used:  
Using all 3 tables in .csv format

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

##### 1️⃣ Empathize  

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_1_5w1h_1.png)

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_1_5w1h_2.png)

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_1_empathy_map.png)

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_1_stakeholde_need.png)

#### 2️⃣ Define point of view  

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_2_define_pov.png)  

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_2_north_star_metric.png)

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/Design%20Thinking/stage_2_growth_formula.png)

#### 3️⃣ Ideate  
#### 4️⃣ Prototype and review  

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Dashboard 1 Preview  

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/overview.png)  

#### 👁️ Observation:

*Click on each photo for closer look*

| 2011 | 2012 | 2013 | 2014 |  
|-------------|----------|-------------|-------------|
| ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/overview_2011.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/overview_2012.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/overview_2013.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/overview_2014.png) |

1. ⌚ Time:  
 - Sales grew steadily from **$2.26M in 2011** to **$4.3M in 2014** — an increase of about **90%**.
 - **Profit** rose from **$248.96K in 2011** to **$504.17K in 2014** — more than **doubling** over the period.
 - **Profit margin** remained stable, moving from **11% to 11.9%**, indicating consistent profitability — a positive sign for sustainable business performance.
 - From **August** to **December**, both Profit and Revenue increased. This growth was driven by:
   - August being a demand-boosting period to stimulate consumer spending.
   - The year-end holiday season, when consumers tend to spend more.
   - September often marking the launch of new product models, prompting higher purchase activity.

2. 🗂️ Segment
 - The **Consumer** segment consistently accounts for the largest share (**47%–54%** each year) → this segment remains the primary focus to drive profitability for the company.
 - The **Corporate** segment ranks second **(~28%–34%)**, followed by **Home Office** with the smallest share.

3. 🏞️ Region
 - Regions with high **Profit Margins** include **Canada (21%–30%)**, **North Asia (18.3%–20.8%)**, and **Central Asia (16.9%–18.3%)**. Canada shows strong potential for market expansion, while North Asia and Central Asia are worth considering for further investment.
 - **Central US** consistently generates the highest absolute **Profit** across years; however, its **Profit Margin** remains at an average level → optimizing costs could further improve profitability.
 - **SEA** and **EMEA** are the weakest performers, showing both low **Profit Margin** and low Profit over the years → these regions should not be prioritized for expansion at this stage.  

#### ✔️ Recommendation:
-> With steady year-over-year growth in **Sales and Profit**, along with stable **Profit Margins**, the company is on a healthy growth trajectory. Departments should continue to sustain this momentum to maintain stable performance.  
-> The **Consumer segment** remains the key focus as it generates the highest profitability for the company. However, it is also recommended to introduce targeted promotions or special offers for **Corporate** and **Home Office** customers to maximize overall revenue.  
-> On the regional side:  
- **SEA** and **EMEA** should be reconsidered for further expansion, as both deliver relatively low Profit.  
- **Canada** deserves attention: while its **Profit Margin** is high, its total **Profit** remains the lowest among regions.  
- **North Asia** and **Central Asia** stand out as attractive opportunities for investment thanks to consistent **Profit Margins (16%–20%)** and relatively strong **Total Profit** compared to other regions.  

#### 2️⃣ Dashboard 2 Preview  

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/region.png)  
  
#### 👁️ Observation:

*Click on each photo for closer look*

| Total Profit | Canada | Central Asia | Southeast Asia | North Asia | Central US | EMEA |  
|-------------|----------|-------------|-------------|-------------|-------------|-------------|
| ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/region_total_profit.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/region_canada.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/region_central_asia.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/region_southeast_asia.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/region_north_asia.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/region_central_us.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/region_emea.png) |

- **Canada** remains the region with the highest **Profit ($17,817.39 at 21.02%)**, followed by **North Asia ($165,578.42 at 16.33%)** and **Central Asia ($132,480.19 at 14.96%)**.
- In terms of **Total Revenue**, Canada ranks last **($66,928.17)**. **Central US** leads with nearly **$3M**, while **North Asia ($848,309.78)** and **Central Asia ($752,826.57)** are both under $1M.
- Looking at **Profit Margin** by product category, Canada is the most balanced across **Furniture (24.7%)**, **Office Supplies (26.5%)**, and **Technology (27.6%)**. North Asia and Central Asia show slightly lower but still solid margins (all above 15%). By contrast, **Central US** and **Southeast Asia** report **negative margins** in **Furniture**, while **EMEA** shows consistent margins across all three product groups.
- **North Asia** records the highest **Return Rate (13.8%)**. For **Canada**, **Africa**, and **EMEA**, return data is missing. **Central Asia (2.3%)**, **Caribbean (2.9%)**, and **South US (2.9%)** have the lowest return rates.
- **Canada** and **South US** both show relatively low **Total Orders** (**201 and 822**, respectively, from 2011–2014). On the other hand, **Central EU (2,576 orders)**, **EMEA (2,462 orders)**, and **Africa (2,232 orders)** lead in total order volume.  

#### ✔️ Recommendation:

- Based on the data, the **US** can be considered a strong candidate for short-term expansion. Its **Total Sales**, **Total Profit**, and **Return Rate** are all stable, making it suitable for near-term investment.  
- For the **medium term**, **North Asia** and **Central Asia** present good opportunities. Strategic approaches such as **flexible pricing** and **operational cost optimization** could further enhance performance in these regions.  
- In the long term, **LATAM (South and Central America)** could be explored through **small-scale pilot** projects before committing fully. The company should gradually build logistics networks to support customers, while running **demand-stimulation** campaigns to test market response and customer behavior prior to a full-scale entry.  

#### 3️⃣ Dashboard 3 Preview  

![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/product.png)

#### 👁️ Observation:

*Click on each photo for closer look*

| Cisco Smart Phone, Full Size | Motorola Smart Phone, Full Size | Nokia Smart Phone, Full Size | Canon imageCLASS 2200 Advanced Copier | Apple Smart Phone | 
|-------------|----------|-------------|-------------|-------------|
| ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/product_cisco_smart_phone.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/product_motorola_smart_phone.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/product_nokia_smart_phone.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/product_canon.png) | ![](https://github.com/longnguyen0102/photo/blob/main/SuperStore-power-bi/product_apple_smart_phone.png) |

- Products in the **Technology** category dominate with **Total Sales of $4.7M**, **Total Profit of $0.7M**, and **Total Revenue of $4.7M**. At least 4 products from this group are among the Top 7 contributors to Profit, Sales, and Revenue. While **Office Supplies** and **Furniture** generate similar Sales and Revenue, Office Supplies delivers higher Profit **($0.5M vs. $0.3M)**.  
- **"Cisco Smart Phone, Full Size"**, **"Motorola Smart Phone, Full Size"**, and **"Nokia Smart Phone, Full Size"** are in the Top 7 for Profit, Sales, and Revenue. These are **"Star products"** (high Sales and high Profit) that the company should focus on defending and expanding market share.
- **"Canon imageCLASS 2200 Advanced Copier"** ranks **#1 in Profit** but only **#5 in Sales** → marketing efforts should be increased to boost its sales. However, attention is required as it has **a high Return Rate (20%)**.
- **"Apple Smart Phone"** leads in **Sales and Revenue**, but does not appear in the **Top Profit** list. To continue selling this product, the company should **optimize cost structure** or **adjust pricing** to improve profitability.

#### ✔️ Recommendation:

-> **Technology** remains the key product category for the company, as it generates both high revenue and profit. The other two categories also require tailored strategies to maximize revenue contribution.  
-> Within the **Top 7 products**, **4–5 are from the Technology group**, reinforcing its strategic importance. Products such as **"Cisco Smart Phone, Full Size"**, **"Motorola Smart Phone"**, and **"Nokia Smart Phone, Full Size"** can be positioned as strategic core products.  
-> Other products like **"Canon imageCLASS"** or **"Apple Smart Phone"** could also serve as flagship offerings if the company implements strategies to optimize pricing, such as:  
- Offering **special promotions** or **customer incentives** for these products.  
- **Negotiating with suppliers** to secure lower procurement costs, enabling more competitive pricing.  

---

## 🔎 Final Conclusion & Recommendations  

👉🏻 Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following:  

📌 Key Takeaways:  
✔️ Recommendation 1  
✔️ Recommendation 2  
✔️ Recommendation 3
