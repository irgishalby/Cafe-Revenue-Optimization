# ☕ Cafe-Revenue-Optimization
**An Exploratory Data Analysis (EDA) for Strategic Decision-Making**

---

## 1. Project Overview

**Café Revenue Optimization** is a data analytics project designed to uncover actionable financial insights from 13 months of café transaction data.  
The goal is to move beyond simple reporting and toward **data-driven decision-making** — identifying key revenue trends, payment behavior, and product performance to support better operational and financial strategies.

The analysis is conducted entirely in **Python (Google Colab)** using the following libraries:
- `pandas` for data manipulation  
- `matplotlib` and `seaborn` for data visualization  

This project produces a **portfolio-ready notebook** that demonstrates end-to-end analytical reasoning and clear business storytelling.

---

## 2. Dataset and Methodology

### 2.1 Data Source

Two CSV files (`index_1.csv` and `index_2.csv`) were merged to create a complete dataset containing transactional records.  
Each transaction includes:

| Column | Description |
|---------|--------------|
| `datetime` | Exact time of the transaction |
| `money` → `revenue` | Transaction amount |
| `coffee_name` → `product` | Coffee or item purchased |
| `cash_type` → `payment_type` | Payment method (Cash or Card) |

---

### 2.2 Analytical Phases

| **Phase** | **Goal** | **Key Actions** |
|------------|-----------|-----------------|
| **Data Cleaning & Engineering** | Ensure accuracy and prepare for time-based analysis | Merged files, removed duplicates, standardized product names, converted datetime strings, and extracted hour/day/month features |
| **Exploratory Data Analysis (EDA)** | Establish key metrics and trends | Calculated total revenue, ARPT (Average Revenue per Transaction), visualized monthly revenue, payment types, and product performance |
| **Advanced Analysis** | Link sales volume with profitability | Computed average price per product and compared to volume to identify pricing opportunities |
| **Conclusion & Recommendations** | Translate analysis into business action | Created an executive summary with strategic recommendations for marketing, staffing, and pricing |

---

## 3. Key Findings and Business Recommendations

### 🪙 A. Financial and Seasonal Performance
**Peak Month:** The analysis identified **February** as the highest revenue period, influenced by a seasonal effect tied to **colder weather**, specific February promotions like **Valentine's Day**, or the start of a local holiday/event cycle.
<img width="984" height="584" alt="image" src="https://github.com/user-attachments/assets/19c8f7d5-f2e8-4424-8df3-6ab7d604b6bc" />

**Recommendation:** Launch targeted campaigns and stock seasonal inventory one month before **February** to maximize sales momentum.

---

### 🕒 B. Operational Efficiency and Staffing
**Peak Hours:** Sales activity peaks at **10.00 AM** and followed by the second peak at **4.00 PM**.  
**Payment Type:** **95.7%** of transactions are paid via **Card**.

**Recommendation:** Align staff scheduling with peak hours to reduce wait times and improve service efficiency.  
Given the high share of digital payments, consider minimizing cash handling and optimizing POS systems for speed.

---

### ☕ C. Product Strategy and Profitability
**Best Seller:** **Americano with milk** generates the highest sales volume at an average price of **$30.39**, serving as a key traffic driver.

**Recommendation:** Implement **upselling strategies** (e.g., pairing with pastries or specialty upgrades) to lift **Average Revenue per Transaction (ARPT)** while leveraging product popularity.
