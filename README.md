
# 📊 Customer Behavior Analytics Dashboard

A Power BI dashboard analyzing **3,900 customer transactions** to uncover product performance, seasonal trends, geographic distribution, and customer segmentation insights. Built to support data-driven decisions in retail fashion.

---

## 📌 Project Overview

Retail businesses collect vast amounts of customer data, but turning it into actionable insights is the real challenge. This dashboard was built to answer critical business questions — from identifying retention risks to optimizing inventory and re-aligning customer loyalty tiers.

The analysis reveals a **critical retention problem**: every customer in the dataset buys exactly once, signaling either 100% churn or a broken repeat-purchase funnel.

---

## 🎯 Objectives

- Analyze overall business performance through KPIs
- Identify top-performing products and seasonal trends
- Evaluate geographic revenue distribution
- Segment customers by behavior and spend
- Assess inventory alignment with seasonal demand
- Validate customer classification accuracy
- Present actionable insights through interactive visualizations

---

## 📂 Dataset

- **Source:** Public customer shopping behavior dataset
- **Format:** CSV
- **Records:** 3,900 transactions
- **Unique Customers:** 3,900 (100% distinct)

The dataset contains customer demographics, purchase details, product categories, seasonal flags, shipping preferences, payment methods, and pre-calculated segmentation fields.

| Field | Description |
|-------|-------------|
| CustomerId | Unique customer identifier |
| Age / AgeGroup | Customer age and bracket |
| ItemPurchased / Category / Size / Color | Product details |
| PurchaseAmount | Transaction value |
| Location | US state |
| Season / SeasonalityFlag | Purchase season and alignment |
| Review Rating | Product rating (1-5) |
| ShippingType / PaymentMethod | Fulfillment and payment |
| PreviousPurchases | Historical purchase count |
| PurchaseFrequency | Self-reported frequency |
| CustomerType / SpendCategory | Behavioral segmentation |

---

## 🛠️ Tools & Technologies

- Power BI Desktop
- Power BI Service (for live sharing)
- Power Query (data cleaning & transformation)
- DAX (measures & calculated columns)
- Data Modeling (star schema)
- Conditional Formatting & Data Bars
- Top N Filtering
- 100% Stacked Column Charts
- Matrix Visuals
- Insight Text Boxes

---

# 📊 Dashboard Pages

## 1️⃣ Executive Summary

High-level KPIs, top products, revenue by season and state, and key performance indicators at a glance.

**Includes:**
- Total Orders (3.90K)
- Total Sales ($233.08K)
- Average Order Value ($59.76)
- Purchase Frequency (1.00)
- Revenue by Season (column chart)
- Top 10 Products (horizontal bar chart)
- Revenue by State (table with data bars)
- Insight text boxes with actionable takeaways

![Executive Summary](Executive%20Summary.png)

---

## 2️⃣ Customer & Season Analysis

Deep-dive into customer segmentation, stocking alignment, and loyalty vs. frequency mismatch.

**Includes:**
- CustomerType × SpendCategory matrix (revenue & transactions)
- Season × SeasonalityFlag matrix (conditional formatting)
- 100% Stacked Column: CustomerType × PurchaseFrequency
- Insight text boxes with strategic recommendations

![Customer & Season Analysis](Customer%20%26%20Season%20Analysis.png)

---

# 📈 Key Performance Indicators

| KPI | Value | Benchmark / Context |
|-----|-------|---------------------|
| Total Orders | 3,900 | Transaction volume |
| Total Sales | $233,081 | Revenue scale |
| Average Order Value | $59.76 | Below fashion benchmark (~$75-100) |
| Purchase Frequency | **1.00** | **100% churn — zero repeat buyers** |
| Unique Customers | 3,900 | No duplicates in dataset |
| Top Product | Blouse ($10,410) | No dominant SKU |
| Peak Season | Fall ($60K) | Only 7% variance across seasons |
| Leading State | Montana ($5,784) | Thin geographic spread |

---

# 💡 Business Questions Answered

### Q1: What is our overall business performance?
**Visual:** KPI cards (Total Orders, Total Sales, AOV, Purchase Frequency)  
**Finding:** $233.08K revenue from 3.90K orders. AOV is $59.76. Purchase Frequency is 1.00 — every customer buys exactly once.  
**Action:** Priority is customer retention, not just acquisition.

---

### Q2: Which products drive the most revenue?
**Visual:** Top 10 Products horizontal bar chart  
**Finding:** Blouse leads at $10.41K, but top 3 are within $90 (Blouse → Shirt → Dress). No dominant SKU.  
**Action:** Bundle top 3 products to increase AOV and create differentiation.

---

### Q3: Which season performs best?
**Visual:** Revenue by Season column chart  
**Finding:** Fall peaks at $60K, but seasonal spread is only ~$4K (7% variance).  
**Action:** Flat seasonality means steady inventory and marketing year-round — no holiday surge needed.

---

### Q4: Which states contribute most?
**Visual:** Revenue by State table with data bars  
**Finding:** Montana leads at $5,784, but top 10 states are within ~$650. Revenue is thinly spread.  
**Action:** Revenue is nationally distributed — deepen in top 3 states before expanding further.

---

### Q5: Who are our most valuable customers?
**Visual:** CustomerType × SpendCategory matrix  
**Finding:** **Frequent customers** drive $139.7K (60% of revenue) with 2,543 transactions. The largest sub-segment is **Frequent Mid Spenders** at $77.9K (33.4%). VIPs underperform at only 16 transactions for $1.5K.  
**Action:** Loyalty program needs attention — VIP tier is not generating expected volume. Realign tiers by behavior, not spend alone.

---

### Q6: Are we stocking right for the season?
**Visual:** Season × SeasonalityFlag matrix with conditional formatting  
**Finding:** Only 24.9% of purchases are "Seasonal Match." Fall and Spring show high match sales ($60K and $58K), but Summer dips to $43K.  
**Action:** Consider off-season promotions or reduce Summer seasonal stock. Investigate why 75% of purchases are off-season.

---

### Q7: Are we classifying customers right?
**Visual:** 100% Stacked Column — CustomerType × PurchaseFrequency  
**Finding:** "Frequent" buyers span Weekly through Annually. VIPs show Quarterly/Annually behavior. The label "Frequent" is misleading.  
**Action:** Realign customer tiers by actual purchase behavior, not spend alone. Annual buyers shouldn't be labeled "Frequent."

---

# ✨ Key Insights

- **🔴 Zero customer retention** — Purchase Frequency = 1.00 indicates every customer is new; 100% churn
- **📉 AOV below benchmark** — $59.76 vs. typical fashion ~$75-100; not extracting full first-visit value
- **🌍 Revenue is flat across seasons** — 7% variance means no seasonal rush strategy needed
- **📍 Geographic spread is thin** — no dominant market; focus depth over breadth
- **🏷️ Customer classification mismatch** — VIPs buy less frequently than "Frequent" tier; labels need rework
- **❄️ 75% off-season purchases** — either seasonal tagging is wrong, or customers ignore seasonality
- **🎯 No product winner** — top 3 products within $90; bundling opportunity exists

---

# 🚀 Features

- Interactive KPI Cards with color-coded thresholds
- Top N Filtering (products, states)
- Conditional Formatting (data bars, background rules)
- 100% Stacked Column Charts (customer classification)
- Matrix Visuals (multi-dimensional segmentation)
- Insight Text Boxes (actionable takeaways below each visual)
- Page Navigation Buttons
- Clean, minimal layout optimized for executive review

---

# 📁 Repository Structure

```
customer-behavior-analytics
│
├── customer_behaviour_analysis.pbix
├── customer_behaviour_analysis.pbit
├── data/
│   ├── cleaned_customer_shopping_behaviour.csv
│   └── customer_shopping_behavior.csv
├── Executive Summary.png
├── Customer & Season Analysis.png
└── README.md
```

---

# 🔮 Future Improvements

- **Cohort Retention Analysis** — track Month 1, 2, 3, 6 repeat purchase rates
- **What-If Parameters** — "If Purchase Frequency rises to 1.20, revenue impact?"
- **Campaign Targets Page** — churn-risk segments for marketing automation
- **Real-Time CRM Integration** — live customer data refresh
- **A/B Test Tracking** — measure retention tactic effectiveness
- **Predictive CLV Model** — identify high-value prospects before first purchase

---

## 👤 Author

**Sehajpreet Kaur**  
Data Analytics & Business Intelligence

- 📧 (sehajpreetkaur5505@gmail.com)
- 💼 (https://www.linkedin.com/in/sehajpreet-kaur-600aa63a0/)

Built as part of my Data Analytics portfolio. Open to freelance projects, feedback, and collaboration.

If you found this project useful, feel free to ⭐ this repository.

