# 🛒 Indian E-Commerce Sales, Discount & Delivery Analysis

> From 8,906 raw orders to clear business answers: what sells, who buys, how deep the discounts go, and whether fast delivery really drives happy customers.

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Colab](https://img.shields.io/badge/Google%20Colab-Notebook-F9AB00?logo=googlecolab&logoColor=white)

---

## 📌 Overview

This project analyses orders from an Indian e-commerce marketplace (December 2020 to October 2021). It combines **Python** for exploration and explanation with a **three-page Power BI dashboard** for interactive viewing, and ends with practical recommendations for the business.

**Questions answered**

1. Which categories, subcategories and brands earn the most?
2. How do sales vary by month and region?
3. How deep are the discounts, and how do prices differ by category?
4. How much does the company earn through commission?
5. How fast and reliable is delivery?
6. Does delivery speed affect customer ratings?

---

## 🔑 Key Findings

| Metric | Result |
|---|---|
| Orders analysed | **8,906** |
| Transaction value | **₹97.40 lakh** |
| Company revenue (commission) | **₹22.17 lakh** (about 22.8% of value) |
| Average discount | **44.3%** (52% of orders get 50% or more off) |
| Average rating | **3.07 / 5** |
| Average delivery time | **2.94 days** (95% of orders take exactly 3 days) |
| On-time delivery | **99.7%** |

**Highlights**

- 📈 **December 2020 was the peak.** 3,369 orders in just 12 days. Per active day, 2020 is 87.6% of the combined daily value against 12.4% for 2021.
- 👗 **Clothing leads** by order count and value. The top 20 subcategories (out of 135) hold about **81%** of value.
- 🌏 **East and West together contribute about 70%** of transaction value. South has the highest average order value.
- 🏷️ **Brand revenue is a long tail.** Of 2,484 brands, 60% have just one order, and the top 10 hold about 24% of brand revenue.
- 🚚 **Delivery is a strength.** It is consistent across regions, years and categories. Delayed orders (4+ days, only 50) rate lower at 2.77, but overall delivery speed has almost no link to rating (correlation about -0.01).

---

## 📊 Power BI Dashboard

**Page 1: Overview**
![Overview](images/Dashboard_Page1_Overview.png)

**Page 2: Pricing, Discounts and Brand Correlation**
![Pricing](images/Dashboard_Page2_Pricing_Discounts_Brands.png)

**Page 3: Rating and Delivery Link**
![Delivery](images/Dashboard_Page3_Rating_Delivery.png)

Every page has year and region slicers. Key DAX measures include Total Orders, Transaction Value, Company Revenue, Average Discount %, On-Time % and Value per Active Day.

---

## 🧪 Approach

1. **Clean:** strip hidden spaces from text columns, check nulls and duplicates (none found), and parse dates with the exact day-month-year format.
2. **Engineer:** add year, month, delivery duration, discount %, company revenue and brand revenue.
3. **Explore:** distributions, category, subcategory, brand and region comparisons, monthly trends, and a brand-level pairplot.
4. **Diagnose:** compare years fairly using value per active day, and relate delivery speed to ratings.
5. **Present:** build the Power BI dashboard and turn the findings into recommendations.

**Commission rule used for company revenue**

| Final price | Commission |
|---|---|
| Above ₹600 | 25% |
| ₹351 to ₹600 | 15% |
| ₹101 to ₹350 | 10% |
| ₹100 or less | 5% |

---

## 💡 Business Recommendations

- Plan stock, marketing and logistics ahead of promotional peaks, using December 2020 as the benchmark.
- Prioritise the top 20 subcategories for stock depth and promotion.
- Review blanket 50% discounts in high-volume categories and test smaller offers.
- Build partnerships with the top brands and offer growth support to long-tail sellers.
- Keep the three-day delivery standard, investigate the 50 delayed orders, and look at product quality and service to lift ratings.

---

## 🧩 Challenges Solved

- **Date parsing:** day-first dates were read as month-first by automatic parsing, producing negative delivery times. Using `format="%d-%m-%Y"` gave correct durations of 0 to 7 days.
- **Hidden whitespace:** names like `"East "` split groups in two until cleaned with `.str.strip()`.
- **Uneven time coverage:** 2020 has 12 order days and 2021 has 115, so years are compared per active day.
- **Small groups:** category averages use only categories with at least 30 orders.

---

## 🗂️ Repository Structure

```
├── data/
│   ├── E-commerce_dt.csv                  # raw data
│   └── PowerBI_Ready_Ecommerce_Data.csv   # cleaned export for Power BI
├── notebook/
│   └── ecommerce_analysis.ipynb           # Python analysis (Google Colab)
├── dashboard/
│   └── ecommerce_dashboard.pbix           # Power BI file
├── images/                                # dashboard screenshots
├── docs/
│   └── Project_Documentation.docx         # full written report
└── README.md
```

---

## ▶️ How to Run

```bash
git clone <your-repo-url>
cd <your-repo-folder>
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook notebook/ecommerce_analysis.ipynb
```

Or open the notebook directly in **Google Colab** and upload the CSV from the `data` folder.

---

## 🔭 Scope and Future Work

The analysis covers Dec 2020 to Oct 2021 and is descriptive and diagnostic. Next steps:

- Statistical tests, for example comparing ratings of delayed and on-time orders
- Demand forecasting with a longer time span
- Customer-level analysis such as repeat purchases

---

## 🛠️ Tools

Python (Pandas, NumPy, Matplotlib, Seaborn) · Google Colab · Power BI (Power Query, DAX) · Excel

---

## 👤 Author

**Bharat Kumaar R**
Data Analyst · Chennai, India
🔗 [LinkedIn](https://www.linkedin.com/in/bharat-rbk25)

If you found this project useful, a ⭐ on the repository is appreciated.
