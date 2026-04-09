# 🛍️ Customer Shopping Behavior Analysis

## 📌 Project Overview
This project focuses on analyzing customer shopping behavior using transactional data from 3,900 purchases across various product categories. The main objective is to uncover meaningful insights into customer spending patterns, segmentation, product preferences, and subscription behavior. These insights can help businesses make informed and strategic decisions.

---

## 📊 Dataset Summary
The dataset consists of 3,900 rows and 18 columns, covering a wide range of customer and transaction-related information.

### Key Features:
- Customer demographics such as Age, Gender, Location, and Subscription Status  
- Purchase details including Item Purchased, Category, Purchase Amount, Season, Size, and Color  
- Shopping behavior data such as Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, and Shipping Type  

There were 37 missing values found in the Review Rating column, which were handled during data cleaning.

---

## 🐍 Exploratory Data Analysis (Python)

The data analysis process began with data cleaning and preparation using Python.

### Data Preparation:
The dataset was loaded using the Pandas library. Initial exploration was performed using functions like `.info()` and `.describe()` to understand the structure and summary statistics.

### Data Cleaning:
Missing values in the Review Rating column were handled using median imputation based on product categories. Column names were standardized into snake_case format for better readability.

### Feature Engineering:
New features were created to enhance analysis:
- Age groups were created by binning customer ages  
- Purchase frequency was converted into days  

### Data Validation:
A consistency check revealed that the `promo_code_used` column was redundant, so it was removed.

### Database Integration:
The cleaned dataset was then connected to PostgreSQL and stored for further SQL-based analysis.

---

## 🧠 SQL Analysis (Business Insights)

SQL was used to extract meaningful business insights from the cleaned dataset. The following key analyses were performed:

- Revenue comparison between male and female customers  
- Identification of high-spending customers who used discounts  
- Top 5 products based on average review ratings  
- Comparison of average purchase amounts between Standard and Express shipping  
- Analysis of subscribers vs non-subscribers in terms of revenue and spending  
- Identification of products highly dependent on discounts  
- Customer segmentation into New, Returning, and Loyal categories  
- Top 3 most purchased products in each category  
- Analysis of repeat buyers and their subscription behavior  
- Revenue contribution by different age groups  

These analyses helped uncover patterns in customer behavior and purchasing trends.

---

## 📈 Power BI Dashboard

An interactive dashboard was created using Power BI to visually represent the insights derived from the data.

The dashboard includes:
- Total number of customers (3.9K)  
- Average purchase amount (~59.76)  
- Average review rating (3.75)  
- Revenue distribution by category  
- Customer segmentation and subscription insights  
- Sales analysis by age group  

This dashboard enables easy interpretation of complex data and supports decision-making.

---

## 📸 Dashboard Preview
<img src="images/dashboard_images/Screenshot 2024-12-15 195004.png" alt="Dashboard" width="800"/>

## 💡 Business Recommendations

Based on the analysis, the following recommendations were made:

- Boost subscription adoption by offering exclusive benefits to subscribers  
- Introduce customer loyalty programs to retain repeat buyers  
- Optimize discount strategies to maintain profitability while increasing sales  
- Highlight top-rated and best-selling products in marketing campaigns  
- Focus marketing efforts on high-revenue age groups and express shipping users  

---

## 🛠️ Tech Stack

- Python (Pandas, Data Analysis, Data Cleaning)  
- SQL (PostgreSQL)  
- Power BI (Data Visualization and Dashboarding)  

---

