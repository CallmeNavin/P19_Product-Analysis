# P19_Product-Analysis

**VERSION 1**

**A. Project Overview**

- This project analyzes user behavioral data from an e-commerce platform to measure Daily Active Users (DAU) and conversion funnel metrics.


![Dashboard Visualization](https://github.com/CallmeNavin/P19_Product-Analysis/blob/main/Version%201/Visualization/Dashboard.jpg)
_Explore more insights in the full Power BI dashboard_

**B. Dataset Information**

_**Source**_

- Retailrocket recommender system dataset (from Kaggle)
- https://www.kaggle.com/datasets/retailrocket/ecommerce-dataset
- In this version, I used only file "events" for analyzing User behaviorals and keep 'Timestamp' columns from September 1st, 2015 to October 31st, 2015
- Due to file size constraints, raw data cannot be uploaded here. Please refer to the Kaggle source link above to download the original dataset if needed.

**C. Methodology**

- Data Cleaning:
  + Filtered events table to keep data from Sept 1–Oct 31, 2015 (final dataset contains only Sept 1–18).
  + Blank Checking:
    - category_tree:
      + Parentid: ~1.5% missing values --> minimal (~1.5%) and correspond to root-level categories without a parent. As no category dictionary is provided in the public dataset, these NaN values are considered expected and require no imputation.
    - events:
      + Transactionid: 99.2% missing values --> Hợp lý. Because blanks occur by design since only transaction events generate an ID, while view and addtocart remain empty.
  + Outliers Checking: 0%
- Export Cleaned Data

**D. Key Findings & Actionable Plans**

_**Key Findings**_

- DAU fluctuates between 10M–17M during Sept 1–18, 2015. Since the dataset covers only half a month, this pattern should be treated as preliminary.
- While DAU trend is inconclusive due to limited timeframe, funnel metrics provide clear evidence of where to optimize (View → Add-to-Cart).Only 2.6% of viewers added items to cart, while ~25% of add-to-cart actions converted into transactions.
- The main bottleneck lies in the View → Add-to-Cart stage.
- DAU in this snapshot is for illustration only (From September 1st - 18th, 2015) and not enough to conclude long-term trends.

_**Actionable Plans**_

- Short-term: Boost View → Add-to-Cart conversion
  + Display promotions and key value propositions directly on the product view page (free shipping, flash deals, bundles, etc).
  + Implement remarketing campaigns targeting users who viewed but did not add to cart (within 24 hours).
- Long-term: Leverage strong Add-to-Cart → Transaction rate
  + Introduce cross-sell/upsell suggestions during checkout to increase basket size.
  + Simplify checkout flow (reduce steps, support multiple payment methods).

**E. Further Version**

- Version 2: Join with item_properties → Funnel by product dimension.
- Version 3: Join with category_tree + price band → Category & pricing insights.

**About Me**

Hi, I'm Navin (Bao Vy) – an aspiring Data Analyst passionate about turning raw data into actionable business insights. I’m eager to contribute to data-driven decision making and help organizations translate analytics into business impact. For more details, please reach out at:

🌐 LinkedIn: https://www.linkedin.com/in/navin826/

📂 Portfolio: https://github.com/CallmeNavin/
