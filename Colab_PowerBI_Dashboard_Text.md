# Colab: Power BI Dashboard Section (copy and paste)

**How to use this file**
1. In your Colab notebook, scroll to the end (after your last analysis cell).
2. Click **+ Text** to add a new text cell for each block below. Paste the heading and text.
3. To add each picture: in the text cell, click the **image icon** in the cell toolbar (or drag and drop the PNG into the cell). Use the file named in the line that says "Insert image here", then delete that line.
4. The three PNG files are in the same download: `Dashboard_Page1_Overview.png`, `Dashboard_Page2_Pricing_Discounts_Brands.png` and `Dashboard_Page3_Rating_Delivery.png`.

---

<!-- ===== NEW TEXT CELL: Section introduction ===== -->

# Power BI Dashboard

The findings from the Python exploration above were brought together in a three-page Power BI dashboard built on the cleaned dataset. Every page includes year and region filters, so a reader can move from the overall picture to a single region or year in one click. Each visual has a counterpart in the notebook, so the dashboard presents and lets the reader filter what the analysis explored and explained.

- **Page 1:** E-Commerce Dataset Overview
- **Page 2:** Pricing, Discounts and Brand Correlation
- **Page 3:** Rating and Delivery Link

---

<!-- ===== NEW TEXT CELL: Page 1: E-Commerce Dataset Overview ===== -->

## Page 1: E-Commerce Dataset Overview

**[Insert image here: Dashboard_Page1_Overview.png]**

**Explanation**

The first page is the executive summary. The top row of cards shows the headline numbers, and the visuals below show where value comes from by category, month, region and subcategory, along with the value per active day by year.

**Observations**

- The marketplace handled 8,906 orders worth ₹97.40 lakh in transaction value. The company earned ₹22.17 lakh in commission, about 22.8% of that value.
- Customers received an average discount of 44.3%, rated their orders 3.07 out of 5 on average, and received them in 2.94 days, with 99.7% delivered on or before the expected date.
- Clothing is the largest category by transaction value, followed by Home Decor, Automotive, Computers and Mobiles and Accessories. At subcategory level, Women's Clothing (₹11.91 lakh), Accessories and Spare Parts (₹11.11 lakh) and Tablet Accessories (₹7.86 lakh) lead. The top 10 subcategories hold about 65% of value and the top 20 about 81%.
- December 2020 is the peak month at ₹41.26 lakh from 3,369 orders. Value falls to ₹23.22 lakh in January 2021, dips to ₹1.81 lakh in February, recovers to ₹14.92 lakh in March and then eases. Order volume from July to October 2021 is very small.
- The value per active day chart shows 2020 at 87.6% and 2021 at 12.4% of the combined daily value, because all 3,369 orders of 2020 were placed on 12 days in December, while 2021 orders are spread over 115 days.
- East contributes 38.67% of transaction value (₹37.7 lakh), West 31.15% (₹30.3 lakh), North 18.71% (₹18.2 lakh) and South 11.47% (₹11.2 lakh).
- In the region by month revenue table, company revenue in December 2020 was ₹9.56 lakh and in January 2021 ₹5.13 lakh. East leads in most months, and West is slightly ahead in February 2021.

**Conclusion**

Performance is shaped by a strong promotional burst in December 2020, a concentrated set of categories and subcategories, and a regional mix led by East and West. The company keeps roughly a fifth of every rupee transacted.

**Business suggestions**

- Plan inventory, marketing spend and logistics capacity ahead of promotional peaks, using December 2020 as the benchmark.
- Give the top 20 subcategories priority for stock depth, search placement and promotion, since they carry about four-fifths of value.
- Use East and West as the base for scale, and treat North and South as growth markets with targeted regional campaigns.
- Track value per active day alongside monthly totals, so that promotional days and normal days can be compared fairly.

---

<!-- ===== NEW TEXT CELL: Page 2: Pricing, Discounts and Brand Correlation ===== -->

## Page 2: Pricing, Discounts and Brand Correlation

**[Insert image here: Dashboard_Page2_Pricing_Discounts_Brands.png]**

**Explanation**

The second page looks at how products are priced and discounted, how retail and discounted prices move together, and which brands earn the most for the company.

**Observations**

- Discounting is the norm: 91.3% of orders carry a discount. The largest group is the 50 to 74% band with 4,297 orders, followed by 25 to 49% (2,360), under 25% (1,125), no discount (775) and 75% or more (349). Overall, 52% of orders carry 50% or more off.
- The category table shows an overall average discounted price of ₹1,093.70 against an average retail price of ₹1,969.97, with an average discount of 44.3%.
- Average discounted price differs widely between categories. Furniture is the highest at about ₹10,500, while Pet Supplies, Watches and Clothing sit at the lower end of the price range.
- Discount depth also differs by category. Automotive (about 55%) and Watches (about 57%) are discounted most, while Furniture, Tools and Hardware, Pens and Stationery and Cameras and Accessories are discounted least (roughly 20 to 30%).
- Comparing 2020 with 2021 across the categories that have enough orders, the average order value moved from ₹1,225 to ₹1,014 and the average discount from 45.1% to 43.7%.
- The retail versus discounted price scatter shows a strong positive relationship (correlation about 0.94). Categories with higher retail prices also have higher discounted prices, and Furniture stands apart at the high-price end.
- ALLURE AUTO is the leading brand by brand revenue (about ₹4.98 lakh from 469 orders), followed by GAGA (₹2.37 lakh), SLIM (₹2.12 lakh), DAILYOBJECTS (₹1.82 lakh) and DIVINITI (₹1.43 lakh). The top 10 brands hold about 24% of brand revenue across 2,484 brands.

**Conclusion**

Deep, broad discounting is a defining feature of this marketplace. Prices follow a consistent pattern in which the discounted price tracks the retail price, categories differ clearly in how much discount they carry, and brand revenue is led by a few names with a long tail behind them.

**Business suggestions**

- Review blanket 50% offers in high-volume categories such as Clothing and Automotive, and test smaller discounts to see how demand responds.
- Protect margin in high-ticket categories such as Furniture and Computers, where discounts are already lower and each order is worth much more.
- Build account plans for the top brands (ALLURE AUTO, GAGA, SLIM, DAILYOBJECTS, DIVINITI) with joint promotions and priority listing.
- Offer long-tail brands a simple programme, such as seller training or bundled campaigns, to help more of them grow beyond a single order.

---

<!-- ===== NEW TEXT CELL: Page 3: Rating and Delivery Link ===== -->

## Page 3: Rating and Delivery Link

**[Insert image here: Dashboard_Page3_Rating_Delivery.png]**

**Explanation**

The third page evaluates delivery performance and tests whether delivery speed is linked to customer ratings, with filters for region and year.

**Observations**

- Delivery is reliable: 99.7% of orders arrived on or before the expected date, the average delivery time is 2.94 days, and only 50 orders (0.6%) took four days or more.
- Delivery is highly uniform. 8,482 orders (95%) took exactly 3 days, and the rest are spread across 0 days (7 orders), 1 day (223), 2 days (144) and 4 to 7 days (50).
- Average rating is 3.09 for Express (0 to 1 day), 3.07 for Standard (3 days) and 3.06 for Fast (2 days) orders, and 2.77 for Delayed (4 days or more) orders.
- Average delivery time is about 2.9 to 3.0 days in every region and in both years, with differences of less than 0.1 day between regions or years.
- Across product categories, average delivery time is close to 3 days. Cameras and Accessories is the fastest at about 2.6 days. Food and Nutrition shows 3.5 days, but this is based on only two orders.
- Across all orders, delivery days and rating show almost no relationship (correlation about -0.01).

**Conclusion**

Delivery is a strength of the operation. It is fast, consistent across regions, years and categories, and it does not by itself explain how customers rate their purchases. Only the small group of delayed orders shows a lower average rating.

**Business suggestions**

- Keep the three-day delivery standard and use it as a selling point in marketing and on product pages.
- Review the 50 delayed orders by seller, route and category to find shared causes and prevent repeats, since these are the orders with the lowest ratings.
- Because delivery speed does not move ratings much, look at product quality, product description accuracy and after-sales service to improve customer satisfaction.
- Add a short follow-up survey after delivery to understand what drives ratings beyond speed.

---

<!-- ===== NEW TEXT CELL: Overall conclusion ===== -->

## Overall Conclusion

The analysis shows a marketplace driven by promotional peaks, concentrated in a few categories and brands, and built on deep discounting. Delivery is fast, uniform and reliable, and it does not by itself explain customer ratings. The company keeps about a fifth of transaction value as commission, mainly from orders above ₹600.

Looking ahead, sustainable growth is most likely to come from managing discount depth, backing high-ticket categories and the best brands, and planning capacity around peaks.

## Scope

- **Period and size:** 8,906 orders from 1 December 2020 to 24 October 2021, across four regions and 26 product categories.
- **Time coverage:** 2020 contains order activity from 12 days in December and volume from July to October 2021 is low, so year comparisons use value per active day.
- **Small groups:** categories with very few orders (for example Food and Nutrition) are not used for category-level conclusions.
- **Revenue:** company revenue follows the commission slab rule and excludes costs.
- **Future scope:** statistical tests such as comparing ratings of delayed and on-time orders, demand forecasting, and customer-level analysis.
