# P19_Product-Analysis

**VERSION 1**

**A. Project Overview**

- This project analyzes user behavioral data from an e-commerce platform to measure Daily Active Users (DAU), Monthly Active Users (MAU) and conversion funnel metrics (view → cart → transaction).

**B. Dataset Information**

_**Source**_

- Retailrocket recommender system dataset (from Kaggle)
- https://www.kaggle.com/datasets/retailrocket/ecommerce-dataset
- In this version, I used only file "events" for analyzing User behaviorals and keep 'Timestamp' columns from September 1st, 2015 to October 31st, 2015

**C. Methodology**

- Data Cleaning:
  + Filter file 'event', 'timestamp' column from September 1st, 2015 to October 31st, 2015 for analyzing in this version, reduce the workload storage
  + Blank Checking:
    - category_tree:
      + Parentid: ~1.5% missing values --> minimal (~1.5%) and correspond to root-level categories without a parent. As no category dictionary is provided in the public dataset, these NaN values are considered expected and require no imputation.
    - events:
      + Transactionid: 99.2% missing values --> Hợp lý. Because blanks occur by design since only transaction events generate an ID, while view and addtocart remain empty.
  + Outliers Checking: 0%
- Export Cleaned Data
- Handle 'item_properties' file for further versions

**D. Key Findings & Actionable Plans**

_**Key Findings**_

- x

_**Actionable Plans**_

- x

**E. Further Version**

- Version 2: Join with 'item_properties' file - Funnel analysis by product dimension. (behaviors × product).
- Version 3: Join with 'category_tree' + 'price band' - Deep insights

**About Me**

Hi, I'm Navin (Bao Vy) – an aspiring Data Analyst passionate about turning raw data into actionable business insights. I’m eager to contribute to data-driven decision making and help organizations translate analytics into business impact. For more details, please reach out at:

🌐 LinkedIn: https://www.linkedin.com/in/navin826/

📂 Portfolio: https://github.com/CallmeNavin/
