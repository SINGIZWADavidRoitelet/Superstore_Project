# Superstore Analytics: Customer Segmentation & Sales Prediction

## 📌 Project Overview
This project performs an end-to-end data science workflow on the Global Superstore dataset. The goal is to move beyond basic reporting to uncover deep insights into sales drivers and categorize the customer base into actionable segments using Machine Learning.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn
* **Environment:** Jupyter Notebook

---

## 🔍 Key Findings

### 1. Sales Correlation Analysis
Using a Pearson correlation heatmap, we identified the primary "levers" of revenue:
* **The Product Factor:** `Avg_Sales_Per_Product` is the strongest predictor of total sales, outperforming order volume.
* **Logistical Neutrality:** Surprisingly, `Shipping Duration` has near-zero correlation with Sales, suggesting delivery speed is not currently a primary driver of purchase value.
* **High-Ticket Categories:** The **Technology** category consistently drives higher transaction values compared to Office Supplies.

### 2. Customer Segmentation (K-Means Clustering)
We utilized the **Elbow Method** to determine an optimal $k=3$ for clustering customers based on **Total Sales**, **Order Frequency**, and **Average Order Value**.

#### **Segment Profiles:**
* **High Value Loyal:** Our "Whales." They make high-ticket purchases and drive the majority of revenue.
* **Medium Occasional:** The steady "Bread & Butter" segment with consistent, mid-range spending.
* **Low Value Rare:** One-time shoppers with small baskets; these represent a high churn risk.

---

## 💡 Business Recommendations
* **Retention:** Implement a VIP loyalty program for the **High Value** segment to protect top-tier revenue.
* **Growth:** Create "Product Bundles" for **Medium Occasional** shoppers, pairing high-margin Technology items with everyday Office Supplies.
* **Win-Back:** Launch a re-engagement email campaign for the **Low Value Rare** cluster with targeted discounts.

---

## 🚀 How to Run
1. Clone the repository.
2. Install dependencies: `pip install pandas seaborn scikit-learn matplotlib`
3. Open `Superstore_Sales_Data` in Jupyter Notebook.