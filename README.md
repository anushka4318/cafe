# cafe

Project Vision: Connecting Business Reality with Data

Cafes have always interested me;not just as social spaces, but as fast-moving businesses where small operational gaps can quietly impact revenue.
During peak hours, orders move quickly, staff multitask, and documentation can easily fall behind.

This led me to a fundamental question:

Is the business operating at its full potential, or is the 'busy-ness' of daily operations masking opportunities for growth and refinement?

This project uses a dataset sourced from Kaggle and adapted to simulate a realistic cafe business environment.
I approached it not as a data exercise, but as a business diagnosis treating the dataset like real operational data from a functioning company.

Instead of “fixing” the dataset to make it perfect, I deliberately preserved common real-world issues such as missing totals, incomplete fields, and inconsistent entries. These issues often represent the exact points where businesses lose visibility, control, and revenue.
The goal of this project was to demonstrate how structured analysis can transform messy data into clear insights and actionable strategy.

Strategic Focus Areas
1. Product & Revenue Performance

Analyzing which items drive the most revenue and volume, how much each contributes to overall revenue, and whether the business relies too heavily on a small set of products.

2. Customer & Transaction Behavior

Understanding how payment methods impact transaction patterns and order values, and how Average Order Value (AOV) varies across payment methods and locations.

3. Channel & Operational Performance

Evaluating how In-store vs Takeaway affects product performance, identifying top-performing days of the week, and highlighting operational gaps such as pricing and total mismatches.

4. Time-Based Trends & Growth

Examining monthly sales trends and identifying peak periods and best-performing products to support planning and forecasting.

An interactive Excel dashboard used to report and explore sales trends can be found here [link].

Data Structure and Initial Checks

The main database structure as seen below consists of 1 main table with a total row count of 10,000 records.

<img width="860" height="478" alt="dataset structure" src="https://github.com/user-attachments/assets/8dcdf150-7a57-4f5a-a588-eff7aa9efa3c" />

This is the menu table along with its price per unit value adjacent to the item name.

<img width="146" height="217" alt="menu" src="https://github.com/user-attachments/assets/9f2f0255-b4c1-44c2-93b9-0d39a73eeb21" /> 

Insight Deep Dive
Total Market Capture: The business generated a total audited revenue of $80,347.50. This figure represents the "reclaimed" total after accounting for the 463 missing transaction entries.

The "Wellness Hero" Revenue Anchor: A critical 51% of total revenue is concentrated in just three core categories: Salads, Sandwiches, and Smoothies. These items serve as the brand's financial foundation, driven primarily by their premium price points and strong market fit.

Volume vs. Value Dynamics: From a pure volume perspective, the top three movers are Coffee, Salads, and Cookies. While Coffee and Cookies drive high foot traffic and frequency, their lower price points mean they act as "entry products" compared to the high-value revenue drivers.

The "Product Champion" Analysis: Salads emerge as the undisputed business winner, topping both the revenue and volume charts. With a high Average Order Value (AOV) of $15, this category represents the ideal balance of consumer demand and high-margin contribution.

Operational Visibility Warning: The "Unspecified Category" currently holds the 4th position in total performance with an AOV of $10. This identifies a significant operational failure in transaction logging; a major portion of business value is being captured without being properly attributed to a specific product line.


Customer & Transactional Logic:

The "Blind Spot" in Customer Intelligence: A significant 31% of the total customer base is currently categorized as "Unspecified." This represents a major gap in the business's ability to track loyalty or behavior, effectively leaving nearly a third of our audience as an invisible demographic.

Balanced Channel Engagement: Setting aside the unspecified data, the business shows a remarkably even split between In-store (30.58%) and Takeaway (29.64%) orders. This parity suggests the brand is equally successful as a destination cafe and a convenience-led grab-and-go model.

Operational Capture Friction: The fact that "Unspecified" entries tie with our primary revenue channels is a clear indicator of operational friction. It suggests that during peak transaction periods, the process for logging customer or order types is being bypassed in favor of service speed.

Strategic Channel Resilience: The near-equal distribution between In-store and Takeaway orders provides the business with revenue resilience. The brand is not overly dependent on one single channel, allowing for flexibility in how physical space is allocated or how marketing is targeted.


Operational Integrity & Value Leakage

My investigation into the "Digital Infrastructure" of the business revealed significant friction points where the pace of daily operations has outpaced the system’s ability to capture data. I have categorized these into three specific Operational Blind Spots:

The "Unspecified" Revenue Signal: The "Unspecified" product category holds an Average Order Value (AOV) of $10, ranking it as the 4th highest revenue contributor. This is a major operational red flag; it indicates that a high-value portion of our sales is being pushed through the system without proper categorization, making it impossible to manage inventory or forecast demand for these "ghost" products.

The Revenue Leakage Gap: My forensic audit identified 463 records (representing a significant fiscal percentage) where Quantity and Price Per Unit were logged, but the Total Sales remained unrecorded. This represents direct revenue leakage—value that was created in the kitchen and served to a customer but was effectively "lost" in the final financial reconciliation due to a system sync failure.

Channel & Payment Anonymity: A disproportionately high volume of transactions is being logged with "Unspecified" Location and Payment Method data. This suggests that during peak "rush" hours, staff are likely bypassing these mandatory fields to maintain service speed. While this keeps the line moving, it strips the business of the intelligence needed to decide whether to invest in more In-store seating or more Takeaway kiosks.

Seasonal Velocity & Revenue Cycles

By mapping the 8,997 transactions across a fiscal timeline, I identified a distinct "seasonal heartbeat" for the cafe. Understanding these cycles allows for smarter resource allocation and inventory management.

Consistent Daily Performance: The business demonstrates remarkable stability on a day-to-day basis. Revenue concentration and transaction volume remain consistent across the week, suggesting a loyal, habit-based customer base rather than one driven by erratic weekend surges.


Strategic Recommendations: The Growth Roadmap
Here are your five recommendations, polished to reflect a "Business Architect" persona:

1. Operational Integrity & Data Capture Training
Implement a targeted staff training program focused on "Peak-Hour Data Integrity." By simplifying the POS interface for high-velocity items and mandating Category/Location selection, we can eliminate the $10 AOV "Unspecified" gap and the 463 unrecorded transactions, ensuring every dollar of value is accounted for in the P&L.

2. Seasonal Revenue Leveling (The "Trough" Strategy)
To bridge the revenue dip in February and May, we will launch seasonal-specific campaigns:

February (Winter Warmth): Introduce high-margin hot beverage combos paired with a "Home-Comfort" takeaway discount to drive volume during cold months.

May (Summer Preview): Launch a "Summer Shake & Smoothie" series, utilizing healthy, vibrant combos to spark interest before the peak June season.

3. High-Performance Menu Diversification
Since Salads are the undisputed "Brand Winner" in both volume and AOV ($15), the business should diversify this category. Introducing 1–2 seasonal salad variations leverages existing customer affinity and minimizes the risk of "menu fatigue" for our most loyal demographic.

4. Strategic "Hero" Bundling
Maximize the 80/20 rule by creating an "Elite Wellness Combo" that bundles our three top performers (Salad, Sandwich, and Smoothie) at a slightly lower price point than individual purchases. This simplifies the decision-making process for the customer and guarantees a high-value transaction for the business.

5. High-Volume Incentive Engineering
Utilize Cookies (a high-volume, high-affinity item) as a strategic incentive. By offering a "Free Cookie with any Salad & Drink combo," we can leverage the low cost of the cookie to drive sales of our high-margin "Wellness Heroes," effectively increasing the total transaction value through psychological "reward" marketing.

The "Peak Performance" Windows: June, April, and October emerge as the strategic high-points for the brand, with each month contributing 12.5% to the total annual revenue. During these peak windows, our "Wellness Heroes" (Salads, Sandwiches, and Smoothies) see their highest velocity, confirming that our core product-market fit is strongest during these transition seasons.

Troughs and Contraction Periods: February and May represent the lowest engagement periods, with revenue concentration dipping to just 3.24%. These "trough" months identify a critical business opportunity: the need for seasonal promotions or "limited-time offers" to bridge the gap and maintain cash flow during off-peak times.


Strategic Adjustments & System Guardrails
In any real-world operation, data is rarely perfect. To ensure the integrity of the business simulation and provide a reliable roadmap for growth, I applied specific logical guardrails to account for system inconsistencies:

Financial Reconciliation (Revenue Recovery): For the 463 records where a transaction occurred but no "Total Sales" was recorded, I manually calculated the values using the Quantity × Price Per Unit logic. This adjustment was essential to capture the true $80,347.50 revenue footprint of the business.

Contextual Imputation (Seasonal Continuity): Where specific monthly data points were missing or inconsistent, I utilized historical performance averages from adjacent peak months (June and October) to maintain a continuous trend analysis, ensuring the "Seasonal Velocity" report remained accurate.

Data Integrity Filtering (The 3% Rule): Approximately 3% of the date and quantity entries contained non-sensical or "corrupted" values (e.g., negative quantities or future dates). To prevent these from skewing our Average Order Value (AOV), these outliers were excluded to ensure the findings represent realistic customer behavior.

Attribute Standardization: "Not Noted" or "Unknown" entries in the Location and Payment columns were treated as a distinct category rather than deleted. This allows the business to measure the "Visibility Gap" as an operational metric rather than hiding it as a data error.
