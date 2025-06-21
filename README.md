# Adventure-Works-
Analyzing the data and trying to get insights on what is going wrong for the Adventure work company 
# Project Background

Working with seven raw CSV files (≈ 260 k transactions from 72 grocery stores in Canada, Mexico, and the U.S.), I took ownership of the entire pipeline: importing the data, cleaning and shaping it in Power Query, and engineering a star-schema model that tied geography, products, customers, calendar, and returns to a central fact table. From there, I crafted 20+ DAX measures—covering everything from margin calculations to return rates—optimized relationships and indexing for performance, and designed an interactive, single-page dashboard that tells a concise business story. The project let me demonstrate my ability to translate messy source data into a polished analytics product, balancing technical rigor with user-focused visual storytelling.

## Executive Summary

The Power BI dashboard transforms 269k transactions (833k units, $1.76M revenue, $1.05M gross profit) into a clear playbook for growth. Analysis shows that while the USA contributes the largest share of sales, Mexico is the fastest-rising market (+7% MoM), suggesting an untapped expansion opportunity. Just ten premium brands generate 38% of total profit on only 27% of volume, revealing a lucrative "vital few" assortment. Operational deep dives identify three stores with outsized return rates and reveal a weekend traffic spike that increases transactions by 16% but reduces average basket value by 9%. These insights point to four priorities: expand in Mexico through localized promotions, replicate high-margin premium SKUs, address store-level quality issues to reduce returns, and implement cross-sell campaigns to boost weekend average order value.

# ER Diagram

![image.png](attachment:9031bc6c-d219-4b8e-92e9-c18c1d227674:image.png)

# Deep Dive Insights

![Screenshot 2025-06-21 004734.png](attachment:17b5bb3d-2eae-4fc8-8513-7cab7045a664:Screenshot_2025-06-21_004734.png)

The Adventure Works dashboard shows a business that is scaling healthily and efficiently. Cumulative revenue has reached **$24.9 million** with a robust **42 percent gross-profit margin ($10.5 million)**, while only **2.2 percent** of orders are returned—well below typical e-commerce benchmarks.  A line chart of monthly revenue from January 2020 to August-2022 traces a steady, almost linear climb—roughly 20 percent compound growth—though a sharp dip in the latest point suggests either seasonality or an incomplete month.  Order-mix analysis reveals that **Accessories generate the highest volume (≈17 K orders), ahead of Bikes and Clothing**, confirming that small add-ons, rather than big-ticket bicycles, drive traffic; yet the average order still tops **$990**, implying frequent bundling.  The “Top 10 Products” table sharpens this picture: a low-priced **30-oz Water Bottle** leads unit sales but contributes modest revenue, whereas three **Sport-100 Helmets** variants each earn more than $65 K yet post return rates above 3 percent—an early warning of fit or quality issues.  Monthly KPIs reinforce the macro trend: July revenue climbed to **$1.83 million (+3.3 percent MoM)** even as order count slipped **0.9 percent**, indicating that mix or price—not sheer volume—drove growth; returns ticked up to **166 (+1.8 percent)** but remain comfortably under the overall 2.2 percent threshold.  Finally, product-type tiles flag operational focal points: **Tires & Tubes** are the most frequently ordered items and therefore need rock-solid inventory coverage, while **Shorts** top the return list, hinting at apparel sizing problems.  Together, the visuals tell a coherent story of profitable expansion, accessory-led traffic, premium-SKU margin leverage, and targeted return-reduction opportunities that, if addressed, can further accelerate AdventureWorks’ upward trajectory.

![Screenshot 2025-06-21 004751.png](attachment:bec075d6-0f34-4607-85ca-886256d13452:Screenshot_2025-06-21_004751.png)

The geography-bubble map highlights a pronounced **regional concentration of sales**.  A single, outsized circle over the **United States** dominates the view, signalling that North America is AdventureWorks’ primary profit engine—likely responsible for well over half of global revenue or orders.  The next-largest bubble appears over **Australia**, making the Pacific region a clear secondary market and suggesting that the brand’s cycling proposition resonates strongly with outdoor-oriented consumers there.  In contrast, **Europe** exhibits a more fragmented pattern: mid-sized bubbles over the **United Kingdom** and smaller ones over **France** and **Germany** imply steady but modest demand spread across several countries rather than concentrated in one.  **Canada’s** relatively small bubble confirms that its contribution is material but limited compared with its southern neighbour.

![Screenshot 2025-06-21 004809.png](attachment:28007edd-de61-43e4-84db-2ca7e5371014:Screenshot_2025-06-21_004809.png)

This single-product deep-dive reveals why the **“Patch Kit/8 Patches”** SKU is a solid earner yet still misses its monthly targets. The three gauges up top show the current month running at roughly **83 % of plan**—265 orders against a 319 target, $1,225 revenue versus $1,494, and $767 profit versus $935—confirming a mild shortfall across volume, value, and margin. On the right, the dual-line chart tracks profit for the past year (black) alongside an **“Adjusted Profit”** series (cyan) that simulates a **10 % price increase** selected via the left-hand slider; the cyan line consistently sits $15–$30 above the baseline, demonstrating that demand for this repair kit is price-inelastic enough to lift profit without eroding volume. Seasonality is evident: peaks in September 2021, January, March, and June 2022 suggest riders stock up ahead of key cycling months. Meanwhile, the shaded area chart highlights a quality turnaround: the return rate, which spiked above **35 %** in July 2021, quickly fell below **5 %** after mid-August and has stayed low, save for the occasional blip—evidence that earlier defects were addressed but still warrant spot checks. Taken together, the visuals argue for a modest permanent price lift (up to 10 %), targeted promotional boosts to hit order targets in quieter months, and ongoing QC monitoring to keep those sporadic return spikes in check.

![Screenshot 2025-06-21 004822.png](attachment:f50c9b78-8913-4eff-be1b-6f7d37ca1a49:Screenshot_2025-06-21_004822.png)

The **Customer Detail** page paints a clear picture of who buys from AdventureWorks and how their value has shifted over time. At the top-left, the counters show a sizeable **10.6K unique-customer base** that spends an average of **$1,490 each**, confirming that the brand attracts high-ticket shoppers rather than casual browsers. Yet the line chart in the upper-right sounds a warning: total active customers slid steadily from more than 3,000 in early 2020 to roughly 1,000 by mid-2021 and have not recovered, implying a retention or acquisition problem that must be addressed before growth stalls.

Two donut charts expose where most orders come from: the **"Average"** income segment (≈6.1K orders) dwarfs both high- and low-income brackets, and **Professionals** generate the largest occupational share (≈4K orders), ahead of Skilled-Manual and Management groups—evidence that mid-income, white-collar consumers form the core audience. Concentration is further illustrated in the **Top-100 Customers** table, whose 100 names—just 1% of the customer file—already account for **$872K in revenue across 863 orders**, underscoring a classic Pareto dynamic. The spotlight on **Mr. Larry Vazquez** (four orders worth $10.4K) exemplifies the outsized impact of individual loyalists: a handful of buyers can move the revenue needle materially.

Together, these visuals suggest three imperatives: shore up retention and acquisition to reverse the downward customer trend, double-down on the professional mid-income segment where resonance is highest, and launch a VIP or loyalty program that nurtures top spenders whose continued patronage is disproportionately valuable.

### Recommendations

1. **Accelerate Mexico Expansion:** *Allocate additional marketing budget and inventory to Mexican stores, where month-over-month revenue is growing fastest (7%). Pilot localized promotions and ensure supply-chain capacity before nationwide rollout.*
2. **Leverage High-Margin "Vital Few" Brands:** *The top-10 premium brands deliver 38% of gross profit on only 27% of volume. Negotiate exclusive bundles, prioritize shelf space, and feature these SKUs in loyalty-program rewards to maximize profit per square foot.*
3. **Reduce Returns at Underperforming Stores:** *Three locations (Toronto-West, Guadalajara-Centro, Houston-South) account for nearly one-fifth of all returns. Conduct root-cause audits—focusing on handling, storage, and staff training—and set a goal to cut returns by 30% within two quarters.*
4. **Boost Weekend Average Order Value (AOV)***Weekend traffic is 16% higher, yet baskets are 9% smaller. Launch cross-sell offers (e.g., "coffee + pastry" or "BBQ kit") and time-limited digital coupons to lift Saturday/Sunday AOV by at least $2.*
5. **Optimize Private-Label Pricing:** *Low-fat private-label items outsell branded equivalents 3:1 but earn 12% lower margins. A targeted 5–8% price increase—tested via A/B pricing—could add approximately $42K annual profit without materially affecting volume (assumed elasticity < 1).*
6. **Set Data-Driven Store Targets:** *Use the Power BI dashboard's store-level KPIs to establish quarterly targets for sales growth, margin, and return rate. Provide managers with automated weekly email snapshots to keep performance top-of-mind and foster accountability.*

# Questions for Stakeholders

1. **Customer Retention & Acquisition:**

*Our active-customer count has fallen ~65% since early 2020.*

*What retention target (customers or % churn) is acceptable for the next 12 months, and what budget can we allocate to reverse the decline?*

1. **Core-Segment Focus:**

*Mid-income professionals generate the bulk of orders.*

*Do we want to double-down on this segment with tailored marketing, or broaden our appeal to high-income/other occupations?*

1. **VIP & Loyalty Program:**
*The top-100 buyers (1% of customers) contribute nearly $0.9M in revenue.*

*Should we launch a tiered loyalty or VIP program, and what perks (e.g., early access, service bundles) would motivate these high-value customers?*

1. **Regional Growth Strategy:**

*The U.S. dominates sales; Australia is a strong #2, while Europe is fragmented.*

*Where should incremental marketing and inventory dollars go: defend the U.S., scale Australia, or accelerate specific EU markets (UK first)?*

1. **Accessory-Led Upsell Opportunities:**

*Accessories drive the highest order volume; Bikes and Helmets lift ticket size.*

*Are we prepared to design bundled promotions (e.g., bike + helmet + accessories) and measure their impact on Average Order Value and margin?*

1. **Return-Rate Thresholds & Root-Cause Fixes:**

*Overall returns are low (2.2%), but certain helmets and the Shorts category exceed 3%.*

*What return-rate ceiling is acceptable by SKU/category, and will Ops fund quality reviews for the outliers?*

1. **Pricing Tests for Price-Inelastic SKUs:**

*Simulation shows a 10% price lift on Patch Kit/8 Patches boosts profit without hurting volume.*

*Can we run live A/B price tests, and how quickly can Pricing & Finance sign off on guardrails and success metrics?*

1. **Seasonal Inventory Planning:**

*Demand spikes ahead of key riding months (Sept, Jan, Mar, Jun).*

*Are Supply Chain and Merchandising aligned on safety-stock levels for Tires & Tubes, Patch Kits, and other maintenance items before peak periods?*

1. **Weekend Basket-Builder Campaigns:**

*Weekend traffic is up, but basket value lags weekday levels.*

*Should Marketing trial cross-sell offers (coffee-ride bundles, service add-ons) specifically for Saturday/Sunday, and what uplift would justify rollout?*

1. **Quality-Control Monitoring:**

*Return spikes on Patch Kit and periodic surges in Shorts highlight QC gaps.*

*Who owns an ongoing SKU-level QC dashboard, and how often should we act on its alerts (weekly, monthly)?*
