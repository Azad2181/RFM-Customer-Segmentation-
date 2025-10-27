# RFM-Customer-Segmentation-
This project performs **RFM (Recency, Frequency, Monetary) Segmentation** to categorize customers based on their purchasing behavior.   It helps businesses understand customer value, loyalty, and engagement to design personalized marketing strategies.

---

## 📋 Table of Contents
- [About the Project](#about-the-project)
- [Business Objective](#business-objective)
- [Dataset Description](#dataset-description)
- [RFM Model Overview](#rfm-model-overview)
- [Project Workflow](#project-workflow)
- [Technologies Used](#technologies-used)
- [Installation and Setup](#installation-and-setup)
- [Results and Insights](#results-and-insights)
- [Project Structure](#project-structure)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## 💡 About the Project

Customer segmentation using RFM analysis divides customers into groups based on:
- **Recency (R):** How recently a customer made a purchase.
- **Frequency (F):** How often a customer makes a purchase.
- **Monetary (M):** How much money a customer spends.

This project aims to **identify high-value customers**, **retain loyal buyers**, and **re-engage dormant customers**.

---

## 🎯 Business Objective

The main goal is to **analyze transactional data** and create meaningful **customer segments** for targeted marketing.

For example:
- Reward loyal customers.
- Win back inactive customers.
- Optimize promotions and email campaigns.

---

## 📊 Dataset Description

The dataset contains customer purchase history with columns such as:

| Column Name        | Description |
|--------------------|-------------|
| CustomerID         | Unique customer identifier |
| InvoiceNo          | Unique invoice number |
| InvoiceDate        | Date of transaction |
| Quantity           | Number of items purchased |
| UnitPrice          | Price per item |
| Country            | Customer's country |
| TotalAmount        | Total purchase amount (Quantity × UnitPrice) |

> 💡 You can use your own sales dataset (e.g., from an eCommerce platform or retail system).

---

## 🧠 RFM Model Overview

The RFM Model is based on three key factors:

| Metric | Meaning | Example Calculation |
|--------|----------|---------------------|
| **Recency (R)** | Days since the last purchase | `(Today - LastPurchaseDate)` |
| **Frequency (F)** | Number of transactions | `Count of unique invoices` |
| **Monetary (M)** | Total amount spent | `Sum of total purchase amount` |

After calculating the three metrics, customers are scored and grouped into segments like:
- **Champions**
- **Loyal Customers**
- **Potential Loyalists**
- **At Risk**
- **Hibernating**
- **Lost**

---

## 🧭 Project Workflow

1. **Import Libraries**
   - pandas, numpy, matplotlib, seaborn, datetime, etc.

2. **Load the Dataset**
   - Read data using `pandas.read_csv()` or `read_excel()`.

3. **Data Cleaning**
   - Handle missing values.
   - Remove duplicates.
   - Filter invalid transactions (e.g., negative quantities).

4. **RFM Calculation**
   - Calculate Recency, Frequency, and Monetary for each customer.

5. **RFM Scoring**
   - Assign scores (1–5) for each R, F, and M metric.

6. **RFM Segmentation**
   - Combine scores into a single RFM segment (e.g., 555 = best customers).

7. **Clustering (Optional)**
   - Use **K-Means** or **Hierarchical Clustering** to create advanced segments.

8. **Visualization**
   - Plot histograms, heatmaps, and customer segment distribution.

9. **Export Results**
   - Save the segmented dataset as CSV for marketing or BI tools.

---

## 🛠 Technologies Used

| Category | Tools / Libraries |
|-----------|-------------------|
| **Programming Language** | Python 3.x |
| **Data Analysis** | pandas, numpy |
| **Visualization** | matplotlib, seaborn |
| **Machine Learning (optional)** | scikit-learn |
| **Notebook Environment** | Jupyter Notebook |
| **Version Control** | Git, GitHub |


THNAKS