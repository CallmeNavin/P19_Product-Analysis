# P19_Product-Analysis

**VERSION 1**

**A. Project Overview**

- This project aims to:
  + 1 DAU
  + 1 MAU
  + 1 funnel

**B. Dataset Information**

_**Source**_

- Retailrocket recommender system dataset (from Kaggle)
- https://www.kaggle.com/datasets/retailrocket/ecommerce-dataset
- Sampling Data (Keep 1000 rows/file)

**C. Methodology**

- Combine 2 raw data files: item_properties_part1 & item_properties_part2 into 1 file: item_properties
- Change file "events" into csv for reduct storage, load fast to google colab
- Data Cleaning:
  + Blank Checking:
    - category_tree:
      + Parentid: ~1.5% missing values --> minimal (~1.5%) and correspond to root-level categories without a parent. As no category dictionary is provided in the public dataset, these NaN values are considered expected and require no imputation.
    - events:
      + Transactionid: 99.5% missing values --> Hợp lý. Because blanks occur by design since only transaction events generate an ID, while view and addtocart remain empty.
  + Outliers Checking: 0%

**D. Key Findings & Actionable Plans**

_**Key Findings**_

- x

_**Actionable Plans**_

- x

**E. Appendix**

- x

**About Me**

Hi, I'm Navin (Bao Vy) – an aspiring Data Analyst passionate about turning raw data into actionable business insights. I’m eager to contribute to data-driven decision making and help organizations translate analytics into business impact. For more details, please reach out at:

🌐 LinkedIn: https://www.linkedin.com/in/navin826/

📂 Portfolio: https://github.com/CallmeNavin/
