# Project 1: ASOS Brand Strategy Analysis

This project involved performing an end-to-end data analytics pipeline to derive actionable brand-level insights and identify inventory opportunities from retail data.

## Technical Process & Methodology

* **Data Cleaning & Preprocessing:** 
    * Initiated the process by loading the dataset and implementing a `skip` rule for bad lines to ensure data integrity.
    * Standardized the `price` column by converting it to numeric values and removing rows with missing pricing information.
* **Feature Engineering & Brand Mapping:**
    * Developed a custom `get_brand` function to extract brand names from product description strings.
    * Utilized **Pandas** to create a `brand_map` dictionary, consolidating variant brand names into a unified brand identity.
* **Inventory & Revenue Analysis:**
    * Quantified "phantom revenue loss" by calculating the financial impact of out-of-stock sizes multiplied by the product price.
    * Aggregated data using **Pandas** to identify which brands represent the highest revenue risk due to inventory gaps.
* **Analytical Visualization:**
    * Used **Seaborn** and **Matplotlib** to generate comprehensive visual profiles, including scatterplots mapping Average Price against Stockout Rates.
    * Employed threshold lines to visually isolate brands that represent both high-value and high-stockout risks.

## Strategic Insights

Through this analysis, I identified actionable opportunities for brand optimization:

* **Inventory Optimization:** By pinpointing high-value items with frequent stockouts, the analysis provides a clear target list for replenishment to recover unrealized revenue.
* **Brand Performance Mapping:** The visual analysis effectively segments brands into those requiring urgent stock intervention versus those performing optimally, providing a data-driven foundation for procurement strategies.

# _____________________________________________________________ #
# project:2  Customer Segmentation & Marketing Strategy Analysis

This project involved performing an end-to-end data analytics pipeline to derive actionable marketing insights from consumer data.

## Technical Process & Methodology

*   **Data Cleaning & Preprocessing:** 
    *   Initiated the process by cleaning the raw dataset, which involved removing statistical outliers such as ages over 90 and income levels exceeding 600,000.
    *   Filtered the dataset to remove irrelevant campaign features and noise.
*   **Feature Engineering & Scaling:**
    *   Utilized **Pandas** and **NumPy** for data manipulation and structure.
    *   Applied **Scikit-learn’s `LabelEncoder`** to convert categorical data into numerical formats and used **`StandardScaler`** to normalize all numerical features.
*   **Dimensionality Reduction & Clustering:**
    *   Implemented **Principal Component Analysis (PCA)** via **Scikit-learn** to compress high-dimensional data into three principal components.
    *   Deployed the **K-Means clustering algorithm** and utilized the **Yellowbrick `KElbowVisualizer`** to mathematically identify the optimal number of consumer segments (K=4).
*   **Analytical Visualization:**
    *   Used **Seaborn** and **Matplotlib** to generate comprehensive visual profiles including countplots, scatterplots, and boxenplots.

## Consumer Behavior Insights

Through this analysis, I identified four distinct customer segments:

*   **Cluster 0 (Older Parents):** Teenager-led households; strategy focuses on convenience and multi-buy discounts.
*   **Cluster 1 (Younger Parents):** Small, child-centric households; strategy prioritizes premium, health-focused, and fresh produce.
*   **Cluster 2 (High-Income Couples):** Non-parents with high disposable income; strategy emphasizes gourmet and premium products.
*   **Cluster 3 (Lower-Income Parents):** Large families needing maximum savings; strategy centers on bulk-buying and store-brand value products.
