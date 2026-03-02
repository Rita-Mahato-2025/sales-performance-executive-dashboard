# Sales Performance Dashboard – Power BI
### 🧩 Domain: Insurance
End-to-End Power BI Project | Sales Performance | Revenue Deep Dive and Segmentation

**Live Dashboard:** [Click here]()

---
## 📌 Table of Contents
- <a href="#overview">Project Overview</a>
- <a href="#objectives"> Objectives </a>
- <a href="#business-questions">Business Questions</a>
- <a href="#key-metrics"> Key Metrics </a>
- <a href="#dashboard-features">Dashboard Features</a>
- <a href="#dax-measures">DAX Measures</a>
- <a href="#tools-used">Tools Used</a>
- <a href="#key-insights">Key Insights</a>
- <a href="#dataset">Dataset</a>
- <a href="#author--contact">Author & Contact</a>

---

## 📌 Project Overview
This project analyzes retail sales data to track revenue, transactions, units sold, and customer behavior using Power BI.

## 🎯 Objectives
- Monitor sales performance over time
- Identify high-value customer age groups
- Analyze revenue and units sold by product category
- Support data-driven business decisions

## 🎯 Business Questions
Sales Performance
•	How is the business performing overall?
•	Are sales improving or declining over time?
Customer Demographics
•	What is the customer purchasing behavior?
•	Are customers buying more units or higher priced items?
Product category Analysis
•	Which product category drive the most revenue?
•	Which Categories generate high transaction volume but low revenue?

## 📊 Key Metrics
- Total Revenue
- Total Transactions
- Total Units Sold
- Average Order Value (AOV)

## 📈 Dashboard Features
- KPI cards with summary metrics
- Revenue and transactions trend analysis
- Customer segmentation by age group
- Product category performance analysis
- Interactive slicers for date and age group filtering

## 📈 Important dax-measures

Total Revenue = SUM(retail_sales_dataset[Total Amount])

Total Transactions = DISTINCTCOUNT(retail_sales_dataset[Transaction ID])

Total Units Sold = SUM(retail_sales_dataset[Quantity])

AOV = [Total Revenue] / [Total Transactions]

Max Revenue = 
VAR max_rev = 
MAXX(
    ALL('Date Table'[Month Start]), 
    [Total Revenue]
)
VAR check = if(max_rev = [Total Revenue], max_rev, BLANK())
RETURN
check 

## 🛠 Tools Used
- Power BI
- DAX (Calculated columns & measures)
- Data Modeling & Visualization Best Practices

## 📌 Key Insights
- 46–55 age group contributes the highest revenue
- Seasonal peaks observed in mid-year and Q1 & Q3
- Electronics and Clothing dominate revenue share


## 📂 Dataset
Dummy retail sales dataset created for learning and portfolio purposes.

<h2><a class="anchor" id="author--contact"></a>Author & Contact</h2>

**Rita Mahato** 
Data Analyst  
📧 Email: ds.rita.mahato@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/mahato-rita/)  

