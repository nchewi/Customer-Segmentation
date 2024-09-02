# Customer Segmentation Project

This repository contains files related to my data analysis project.

## Files

- **Jupyter Notebook**: [analysis.ipynb](https://github.com/nchewi/Customer-Segmentation/blob/main/customer_segmentation.ipynb)
  - This notebook contains the code and analysis for the project.

- **Power BI Report**: [report.pbix](https://github.com/nchewi/Customer-Segmentation/blob/main/customer_segmentation.pbix)
  - This file contains the Power BI report. (Download to view)

- **CSV Data**: [transaction.csv](https://github.com/nchewi/Customer-Segmentation/blob/main/transaction_data.csv)
                [customer.csv](https://github.com/nchewi/Customer-Segmentation/blob/main/customer_data.csv)
  - This file contains the dataset used for analysis.

# Customer Segmentation Project

**Nchewi Enya**

## Project Objective

The objective of this project was to segment customers based on their purchasing behavior and demographics to identify distinct customer segments. These segments can then be used to develop targeted marketing strategies, ultimately enhancing customer engagement and optimizing marketing efforts.

## Data Preparation and Clustering

The project utilized two datasets: `customer_data.csv` and `transaction_data.csv`, which contain customer and transaction information.

### Data Cleaning and Transformation

1. **Loading Data:** The dataset was loaded into Python using pandas for data manipulation.
2. **Handling Missing Values:** Missing values were identified and handled through imputation or removal based on the extent of missing data.
3. **Data Type Conversion:** Columns such as “Purchase Date” were converted to appropriate data types.
4. **Feature Engineering:** Derived columns like “Total Spend” were created by multiplying “Quantity” by “Price.”

### Clustering Process

1. **Feature Selection:** Selected relevant features for clustering, including “Age,” “Income,” “Purchase Frequency,” and “Total Spend.”
2. **Normalization:** Standardized the features to ensure that each feature contributed equally to the distance calculations.
3. **Clustering Algorithm:** Applied the K-means clustering algorithm to segment customers into distinct groups.
4. **Cluster Validation:** Evaluated the clusters for validity and coherence using metrics such as silhouette score.

### Cluster Results

The clustering process identified several distinct customer segments. Each segment represents a group of customers with similar purchasing behaviors and demographic characteristics.

## Visualization in Power BI

### Visualizations

1. **Cluster Analysis Visualization:**
   - **Chart Type:** Scatter Plot
   - **X-Axis:** Age
   - **Y-Axis:** Total Spend
   - **Color:** Cluster
   - **Purpose:** This scatter plot visualizes the clusters, showing how different customer segments vary in terms of age and spending. Each color represents a different cluster, helping identify patterns and distinct groupings.

2. **Age Distribution:**
   - **Chart Type:** Column Chart
   - **Axis:** Age
   - **Values:** Count of Customer ID
   - **Purpose:** The column chart shows the distribution of customer ages across different clusters. It helps to identify age group patterns within each segment.

3. **Total Spend by Cluster:**
   - **Chart Type:** Bar Chart
   - **Axis:** Cluster
   - **Values:** Sum of Total Spend
   - **Purpose:** This bar chart illustrates the total spending across different clusters. It highlights the overall spending behavior of each customer segment.

4. **Average Purchase Frequency by Cluster:**
   - **Chart Type:** Column Chart
   - **Axis:** Cluster
   - **Values:** Average of Purchase Frequency
   - **Purpose:** This column chart displays the average purchase frequency for each cluster. It provides insights into how often customers in different segments make purchases.

## Explanation of Clusters

Clustering in data analysis is a technique used to group similar data points together based on their characteristics or features. The main goal of clustering is to identify natural groupings within a dataset so that data points within the same group (or cluster) are more similar to each other than to those in other groups.

### Cluster Characteristics

- **Cluster 0:** Typically younger customers with moderate spending and high purchase frequency. This group might be highly engaged and responsive to promotions.
- **Cluster 1:** Middle-aged customers with high spending but lower purchase frequency. This segment may be more valuable in terms of revenue, suggesting a need for strategies to increase purchase frequency.
- **Cluster 2:** Older customers with low spending and low purchase frequency. This group may require specific strategies to increase engagement or adapt to their purchasing patterns.

### Targeted Marketing Strategies

- **For High-Spending Segments:** Offer loyalty programs and personalized promotions to encourage repeat purchases.
- **For High-Frequency Segments:** Introduce cross-selling opportunities and incentives for increased spending.
- **For Low-Engagement Segments:** Implement targeted campaigns to increase awareness and interest, potentially through special offers or tailored content.

## Conclusion

The project successfully segmented customers based on purchasing behavior and demographics, providing valuable insights into different customer groups. The visualizations created in Power BI offer a comprehensive view of customer segments, enabling the development of targeted marketing strategies to optimize customer engagement and increase revenue. The combination of clustering analysis and visual reporting provides a robust foundation for data-driven decision-making in marketing.

