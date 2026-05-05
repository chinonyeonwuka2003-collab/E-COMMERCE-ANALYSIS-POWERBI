# 📊 Ecommerce Sales Analysis

This repository contains a data analytics project focused on understanding customer purchasing behavior, product performance, and operational efficiency for a retail company.  
The analysis was conducted using **Microsoft Power BI** with DAX measures, dashboards, and visualizations.

---

## 📑 Table of Contents
- [Executive Summary](#executive-summary)
- [Business Problem](#business-problem)
- [Aims & Objectives](#aims--objectives)
- [Data Description](#data-description)
- [Data Preparation & Cleaning](#data-preparation--cleaning)
- [Feature Engineering](#feature-engineering)
- [Methodology](#methodology)
- [Key Findings & Insights](#key-findings--insights)
- [Visualizations](#visualizations)
- [Conclusion](#conclusion)
- [Recommendations](#recommendations)

---

## 📌 Executive Summary
The project analyzes **1,020 sales records** (Jan 2022 – Jan 2023) to uncover revenue drivers, discount impacts, product demand trends, and customer satisfaction insights.  
After cleaning, the dataset contained **889 rows × 18 columns**.

---

## 🛠 Business Problem
Decision‑makers struggle to identify:
- Key revenue drivers  
- Impact of discounts  
- Product demand trends  
- Customer satisfaction insights  

---

## 🎯 Aims & Objectives
1. Identify revenue and profit growth opportunities  
2. Optimize pricing, discounting, and shipping costs  
3. Improve customer retention and experience  
4. Monitor sales performance across categories, locations, and payment methods  

---

## 📂 Data Description
- **Period:** Jan 2022 – Jan 2023  
- **Records:** 1,020 (cleaned to 889)  
- **Columns:** 17 → 18 after cleaning  
- **Key Variables:** Order ID, Customer ID, Product Name, Category, Sub‑Category, Quantity, Price, Discount, Shipping Cost, Total Sales, Payment Method, Order Status, Customer Location, Customer Feedback  

---

## 🧹 Data Preparation & Cleaning
- Removed duplicate Order IDs → 1,000 unique orders  
- Corrected data types (e.g., Order Date → Date)  
- Standardized product names & regrouped categories/subcategories  
- Split State/City into separate columns  
- Recalculated **Total Sales** using:  
  

\[
  \text{Total Sales} = (\text{Quantity} \times \text{Price}) - \text{Discount} + \text{Shipping Cost}
  \]

  
- Replaced missing feedback with `"No Feedback"`

---

## ⚙️ Feature Engineering
- **Processing Speed** = Ship Date – Order Date  
- **Quantity Groups**: High (7–9), Medium (4–6), Low (1–3), Returned (-1)  
- **Shipping Cost Groups**: Low (5–10), Medium (10.03–15), High (15.01–19.99)  
- **Processing Speed Groups**: Same Day (0), Early (1–3), Expected (4–6), Delayed (7–10)  

---

## 📈 Methodology
- Tool: **Microsoft Power BI**  
- Created DAX measures for KPIs: Total Revenue, Total Quantity, Avg Quantity, Customer Count, Avg Processing Speed  
- Built dashboards with 4 pages:  
  - Sales Overview  
  - Customer Behavior & Segmentation  
  - Operational & Shipping Insights  
  - Customer Feedback  

---

## 🔍 Key Findings & Insights
- **Revenue:** $1.05M across 889 orders, 4252 products, 286 customers  
- **Top Product:** Laptop ($190k revenue)  
- **Category Leader:** Electronics  
- **Payment Preference:** Bank Transfer (highest revenue contribution)  
- **Geography:** Arizona generated the most revenue  
- **Customer Loyalty:** Customer 136 is most frequent buyer  
- **Discount Impact:** No clear relationship between discount and sales  

---

## 📊 Visualizations

### Sales Overview Dashboard
!(images/sales_overview.png)<img width="636" height="469" alt="Sales Overview Dashboard" src="https://github.com/user-attachments/assets/f930534b-5475-4f3c-b9a8-52be24b52e5c" />


### Customer Behavior & Segmentation
![Customer Segmentation Dashboard](images/customer_segmentation.png)

### Operational & Shipping Insights
![Operational Insights Dashboard](images/operational_insights.png)

### Customer Feedback
![Customer Feedback Dashboard](images/customer_feedback.png)

*(Replace these placeholders with actual screenshots from Power BI once available.)*

---

## ✅ Conclusion
- Electronics (especially laptops) drive revenue  
- Customers prefer **Bank Transfer**  
- Strong positive relationship between **Quantity & Revenue**  
- Arizona is the top revenue‑generating state  
- Discounts do not significantly boost sales  

---

## 💡 Recommendations
- Reduce prices of underperforming products  
- Tailor regional marketing strategies  
- Improve logistics & delivery processes  
- Investigate recurring negative feedback categories  
- Optimize packaging & logistics for high‑cost items (e.g., laptops)  
- Apply discounts strategically to proven demand products  

---

## 📜 License
This project is for **educational and analytical purposes**.  
Use responsibly and cite appropriately when referencing.
