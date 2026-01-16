# Cafe Data Analysis and Business Strategy

## Project Background

Cafes have always interested me not only as social spaces but as fast-moving businesses where small operational gaps can quietly impact revenue. This project is based on a dataset sourced from Kaggle and adapted to simulate a realistic cafe business environment. I approached this project from the perspective of a data analyst working within the company, treating the dataset as if it were real operational data.

Instead of "fixing" the dataset to make it perfect, I intentionally preserved common real-world issues such as missing totals, incomplete fields, and inconsistent entries. These represent the exact points where businesses often lose visibility, control, and revenue. The purpose of this project is to demonstrate how structured analysis can transform messy, imperfect data into clear insights and actionable business strategy.

Insights and recommendations are provided on the following key areas:

* Category 1: Product & Revenue Performance
* Category 2: Customer & Transaction Behavior
* Category 3: Channel & Operational Performance
* Category 4: Time-Based Trends & Growth

An interactive Excel dashboard used to report and explore sales trends can be found here [link].

---

## Data Structure & Initial Checks

The company’s main database structure consists of 1 primary table with a total row count of 10,000 records. This table represents transaction-level data for the cafe business.

Table 1 (Main Transactions Table):
Contains order-level details such as items sold, quantity, price per unit, total sales, category, location (In-store/Takeaway), payment method, and date fields used throughout the analysis.

Supporting Structure:
A separate menu reference is used, containing item names along with their price per unit values to validate pricing consistency across transactions.

##
<img width="860" height="478" alt="dataset structure" src="https://github.com/user-attachments/assets/b98b7802-ce76-4908-8afe-4bbbb21ad37f" />

##
<img width="146" height="217" alt="menu" src="https://github.com/user-attachments/assets/428fd2a0-136c-4603-8588-bcd4c98f3a50" />



---

## Executive Summary

### Overview of Findings

If a stakeholder were to take away three key insights from this project, they would be:

1. A significant portion of revenue and customer data is being lost due to poor operational data capture (e.g., 463 missing transaction totals and large volumes of "Unspecified" entries).
2. The business’s financial performance is highly driven by a small group of high-performing products (Salads, Sandwiches, and Smoothies contribute 51% of total revenue).
3. The cafe demonstrates strong operational resilience across channels (In-store vs Takeaway) and consistent performance across days, but clear seasonal peaks and troughs require strategic planning.

<img width="856" height="313" alt="category - 1" src="https://github.com/user-attachments/assets/4e60bcbb-9f0d-4d83-9caf-6891f097f1b1" />


---

## Insights Deep Dive

### Category 1: Product & Revenue Performance

Main insight 1: The business generated a total audited revenue of $80,347.50 after recovering value from 463 missing transaction totals. This represents the true financial footprint of the business once data gaps were addressed.

Main insight 2: 51% of total revenue is concentrated in three categories: Salads, Sandwiches, and Smoothies. These products form the brand’s financial foundation due to strong demand and premium pricing.

Main insight 3: From a volume perspective, Coffee, Salads, and Cookies are the top movers. Coffee and Cookies drive high footfall, but their lower price points position them as entry products rather than core revenue drivers.

Main insight 4: Salads emerge as the strongest overall product, ranking highest in both revenue and volume, with an Average Order Value (AOV) of $15. This reflects strong product-market fit and high-margin contribution.

* <img width="675" height="440" alt="cat- 1" src="https://github.com/user-attachments/assets/4af7734d-0ec6-4458-9e9f-cf7233bb5c8b" />


---

### Category 2: Customer & Transaction Behavior

Main insight 1: 31% of customers are labeled as "Unspecified," which represents a major blind spot in customer intelligence and prevents effective tracking of loyalty and behavior.

Main insight 2: Excluding unspecified data, In-store (30.58%) and Takeaway (29.64%) orders are almost evenly split. This shows that the cafe performs equally well as a destination space and as a convenience-led option.

Main insight 3: The high volume of unspecified customer and transaction entries suggests that during peak periods, data capture is being deprioritized in favor of speed of service.

Main insight 4: The balanced split between channels provides strategic resilience, meaning the business is not overly dependent on a single revenue stream.

* <img width="835" height="145" alt="cat 2 better" src="https://github.com/user-attachments/assets/a057f6f6-8b23-4147-96ec-13fbb91f696f" />


---

### Category 3: Channel & Operational Performance

Main insight 1: The "Unspecified" product category ranks 4th in overall performance with an AOV of $10. This is a critical operational red flag, as high-value sales are occurring without being correctly attributed.

Main insight 2: 463 transactions contained quantity and price but were missing total sales values. This represents direct revenue leakage caused by system or process failure during transaction logging.

Main insight 3: A large number of transactions are missing location and payment method details, indicating that staff are likely bypassing mandatory fields during busy periods.

Main insight 4: These operational blind spots do not just affect reporting quality; they directly limit the business’s ability to make informed decisions around staffing, layout, marketing, and investment.


* <img width="583" height="200" alt="operation challege 1" src="https://github.com/user-attachments/assets/e648a158-0050-4341-8f4b-59c471cee943" />

* <img width="928" height="266" alt="cat 2 lost revenue" src="https://github.com/user-attachments/assets/0a15c56f-e49b-4ba7-a486-d23c73f9b9a5" />

---

### Category 4: Time-Based Trends & Growth

Main insight 1: Revenue and transaction volume remain relatively consistent across days of the week, suggesting a loyal, habit-driven customer base rather than heavy weekend dependency.

Main insight 2: June, April, and October each contribute approximately 12.5% of total annual revenue, making them peak performance windows for the business.

Main insight 3: February and May are clear trough periods, with revenue contribution dipping to around 3.24%, highlighting the need for seasonal intervention.

Main insight 4: Product performance during peak months further reinforces that Salads, Sandwiches, and Smoothies have the strongest product-market fit during key seasonal transitions.

[Visualization specific to category 4]

---

## Recommendations

Based on the insights and findings above, we would recommend the leadership and operations team to consider the following:

* A significant amount of value is lost due to incomplete transaction logging. Implement targeted staff training and simplify POS workflows to enforce mandatory category, location, and total capture during peak hours.

* Revenue drops sharply in February and May. Introduce seasonal campaigns such as winter beverage bundles in February and summer-focused smoothie promotions in May to stabilize cash flow.

* Salads are the strongest product across both revenue and demand. Introduce 1–2 seasonal salad variations to deepen engagement with existing loyal customers and prevent menu fatigue.

* The top three revenue drivers (Salads, Sandwiches, Smoothies) can be strategically bundled. Introduce a high-value combo offering to increase average transaction size while simplifying customer decision-making.

* Cookies are a high-volume, low-cost item. Use them as an incentive (e.g., free cookie with premium combo purchases) to psychologically boost perceived value while driving sales of high-margin items.

---

## Assumptions and Caveats

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These are documented below:

* Assumption 1: For the 463 records where Total Sales was missing but Quantity and Price Per Unit were available, Total Sales was calculated manually using Quantity × Price Per Unit to recover true revenue.

* Assumption 2: Where monthly data points were inconsistent or missing, historical averages from adjacent peak months (June and October) were used to maintain continuity in trend analysis.

* Assumption 3: Approximately 3% of records contained nonsensical values (such as negative quantities or future dates). These were excluded from the analysis to prevent distortion of key metrics like Average Order Value.

* Assumption 4: Entries labeled as "Not Noted" or "Unknown" in Location and Payment Method were retained as their own category rather than removed, allowing the visibility gap itself to be measured as an operational metric.
