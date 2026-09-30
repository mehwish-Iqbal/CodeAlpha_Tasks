#   Olist Brazilian E-Commerce Dataset EDA

 **Internship** : CodeAlpha

 **Name** :  Mehwish Iqbal
 
 **Task 01**  : exploratory data analysis 

### 📌 Introduction / Objective

This project was completed as **Task 01 of the CodeAlpha Data Analytics Internship**.

The objective of this task is to perform **Exploratory Data Analysis (EDA)** on the Olist e-commerce dataset to understand sales performance, customer distribution, product categories, order activity, payment behavior, and delivery performance.

The analysis focuses on identifying data quality issues, understanding relationships between different datasets, answering key business questions, and extracting meaningful insights from the data.

---

## 📊 Dataset Overview

This project uses multiple Olist datasets to analyze e-commerce sales, customers, products, payments, and order performance.

### Source Datasets

| Dataset                  |    Rows | Columns |
| ------------------------ | ------: | ------: |
| **Orders**               |  99,441 |       8 |
| **Order Items**          | 112,650 |       7 |
| **Payments**             | 103,886 |       5 |
| **Products**             |  32,951 |       9 |
| **Category Translation** |      71 |       2 |
| **Customers**            |  99,441 |       5 |


### 🔗 Merged Dataset

The relevant datasets were merged using common keys such as `order_id`, `product_id`, and `customer_id` to create a consolidated **`sales_data`** dataset.

**Final Dataset Shape:** `112,650 rows × 16 columns`

This merged dataset was used for the main sales analysis and visualization.


----
## 🛠️ Tools & Libraries

* **Python** — Data analysis and programming

* **Pandas** — Data manipulation and analysis

* **Jupyter Notebook** — Development and analysis environment


The analysis uses multiple datasets from the **Olist Brazilian E-Commerce Dataset**, including:

* Orders
* Order Items
* Payments
* Products
* Customers
* Product Category Translation

These datasets were combined where required to perform a comprehensive analysis.

---

## 🔍 Analysis Performed

### 1. Introduction / Objective

Defined the purpose and business objectives of the exploratory analysis.

### 2. Load Dataset

Loaded the required Olist datasets using **Python and Pandas**.

### 3. Dataset Structure & Data Types

Examined:

* Number of rows and columns
* Column names
* Data types
* Dataset structure
* Basic statistical information

Date-related columns were converted into appropriate datetime formats where required.

### 4. Missing Values Analysis

Identified missing values across the datasets and examined their impact on the analysis.

Missing category information and other incomplete records were investigated and handled appropriately.

### 5. Duplicate Records Check

Checked the datasets for duplicate records to ensure data reliability.

No significant duplicate records were identified in the analyzed datasets.

### 6. Categorical Variables Analysis

Analyzed important categorical variables such as:

* Product categories
* Customer states
* Order status
* Payment types
* Delivery performance

This helped understand the distribution of different business segments.

### 7. Data Quality Issues & Handling

Several data quality issues were identified and addressed, including:

* Missing values
* Unknown product categories
* Inconsistent category information
* Date formatting issues
* Categorical value inconsistencies

Appropriate cleaning and preprocessing steps were applied before conducting the EDA.

### 8. Dataset Relationships / Merging

Multiple Olist datasets were combined using common identifiers such as:

* `order_id`
* `customer_id`
* `product_id`

This allowed sales, customer, product, payment, order, and delivery information to be analyzed together.

---

# 📊 Business Questions & Exploratory Data Analysis

The following business questions were investigated during the analysis.

### 💰 Total Revenue

The total product sales revenue generated across all order items was approximately **$13.59 million**.

This provides a baseline measure of the overall sales performance represented in the dataset.

### 📈 Revenue Over Time

Sales activity was analyzed over time to understand changes in revenue and order activity.

This analysis provides a foundation for identifying potential monthly and seasonal patterns in future visualization work.

### 🛍️ Top Product Categories

Product categories were compared based on revenue contribution.

The highest-revenue categories included:

* **Health & Beauty**
* **Watches & Gifts**
* **Bed, Bath & Table**

These categories made a significant contribution to overall product sales revenue.

### 🧾 Average Order Value

The calculated **Average Order Value (AOV)** was approximately **$137.75**.

This provides an overall indication of the average sales value associated with an order.

### 🗺️ Customer Distribution by State

Customer distribution was analyzed across Brazilian states.

The states with the largest number of customers included:

* **São Paulo (SP)**
* **Rio de Janeiro (RJ)**
* **Minas Gerais (MG)**

São Paulo represented the largest customer base in the dataset.

### 📦 Order Status Distribution

Order statuses were examined to understand the overall order lifecycle.

The majority of orders were **delivered**, while smaller portions were associated with shipped, canceled, unavailable, invoiced, processing, created, and approved statuses.

### 🚚 Delivery Performance

Delivery performance was categorized into:

* On Time
* Late
* Not Delivered

The analysis showed that the majority of analyzed deliveries were completed **On Time**, while a smaller proportion experienced delays or were not delivered.

### 💳 Payment Method Distribution

Payment methods were analyzed to understand customer payment preferences.

The main payment methods included:

* Credit Card
* Boleto
* Voucher
* Debit Card
* Not Defined

**Credit card** was the most frequently used payment method.

### 💵 Payment Value by Payment Method

Payment values were compared across payment methods.

Credit cards accounted for the largest overall payment value  ($12.54M), reflecting their high usage within the dataset.

---

### 📐 Test hypotheses and validate assumptions


**Assumption:** Most orders are delivered on time.

* **H₀:** On-Time and Late delivery proportions are equal.
* **H₁:** On-Time deliveries are higher than Late deliveries.

| Delivery Performance |  Count | Percentage |
| -------------------- | -----: | ---------: |
| **On Time**          | 89,941 | **93.23%** |
| **Late**             |  6,535 |  **6.77%** |

**Chi-Square Test:** `p-value = 0.0`

The result is statistically significant, so **H₀ is rejected**. The data supports the assumption that **most delivered orders are completed On Time**.


---

# 💡 Key EDA Insights / Findings

The exploratory analysis revealed several important findings:

* The dataset represents a large-scale e-commerce operation with approximately **$13.59 million in product sales revenue**.
* **Health & Beauty, Watches & Gifts, and Bed, Bath & Table** were among the leading revenue-generating product categories.
* The average order value was approximately **$137.75**.
* **São Paulo** had the largest customer base among Brazilian states.
* Most orders were successfully **delivered**.
* **Credit cards** were the dominant payment method by both usage and overall payment value.
* Most analyzed deliveries were classified as **On Time**, although late and undelivered orders were also present.
* The statistical analysis indicated a significant relationship between the categorical variables tested in the Chi-Square analysis.

---

# 📝 Conclusion

The Exploratory Data Analysis provided an overall understanding of the Olist e-commerce dataset, including sales, customers, products, orders, payments, and delivery performance.

The analysis identified important patterns in revenue, customer distribution, payment behavior, order activity, and delivery performance. Data cleaning, preprocessing, dataset merging, business-question analysis, and statistical testing provided a strong foundation for understanding the dataset and preparing it for further analysis.

---

# 🔮 Future Analysis / Recommendations

The following areas can be explored in future stages of the project:

* Visualize monthly and seasonal sales trends.
* Compare product category performance using visualizations.
* Explore customer distribution across regions.
* Analyze payment methods and order activity patterns.
* Examine the relationship between product price and freight value.
* Visualize delivery differences across product categories.
* Explore customer reviews through sentiment analysis.
* Develop interactive dashboards for deeper business insights.

---

## 🛠️ Tools & Technologies

* **Python**

* **Pandas**

* **Jupyter Notebook**



---





**Dataset:** Olist Brazilian E-Commerce Dataset

