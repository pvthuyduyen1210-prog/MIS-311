# Part 1: Data Analysis and Insight

**1. Data Overview**

The dataset, titled Cost of Living, was obtained from a global economic database that provides comparative statistics on living expenses and income levels across different regions. It contains **201 rows** and **5 columns**: Country, Year, Average_Monthly_Income, Cost of Living and Region.

Each record represents a country or territory with data collected for a specific year. The dataset aims to highlight variations in cost of living, income levels, and regional economic differences. The main purpose of this analysis is to explore whether higher living costs are associated with higher income levels and to identify global patterns across regions.

**2. Data Cleaning**

The dataset was first cleaned to ensure accuracy and consistency before performing any statistical analysis.
Initially, Excel **TRIM(CLEAN)** formulas were applied to remove all unwanted white spaces and non-printable characters across the dataset, improving readability and preventing data entry inconsistencies.

Next, the dataset was examined for missing values using Excel’s **Filter** feature, with missing cells highlighted for review.
The inspection revealed two missing values in the **Average_Monthly_Income** column and two missing values in the **Region** column.

**To handle these missing values:**

For Average_Monthly_Income, the mean substitution method was used.
The average income across all valid observations was calculated to be 4,243.97 USD, and this value was inserted in place of the two missing records.

For Region, a Pivot Table summarizing Region and Count of Region was created to identify the most frequent region.
The result showed that “North America” appeared most frequently, so this region was used to replace the two missing values.
Region	Count of Region

<img width="680" height="443" alt="Ảnh chụp Màn hình 2025-11-02 lúc 22 20 19" src="https://github.com/user-attachments/assets/3cc16130-ae27-4393-9a4e-61366bb14515" />

Table 1. Frequency Distribution of Regions in the Dataset

Finally, the dataset was checked for duplicate rows, and two duplicates were identified and removed.
After cleaning, the dataset contained **199 complete** and unique rows, with no missing or duplicated data remaining.

**3. Descriptive Statistics**
   
**3.1 Overview of Descriptive Statistics**

Descriptive statistics were employed to explore the central tendencies, dispersion, and distribution of the dataset’s numerical variables. This step helps uncover underlying trends and prepares the foundation for generating meaningful insights.
		

<img width="886" height="443" alt="Ảnh chụp Màn hình 2025-11-02 lúc 22 21 48" src="https://github.com/user-attachments/assets/452eb1fb-274b-450e-a86b-c49cb85ac6ea" />

Table 2. Descriptive Statistics Summary

**3.2 Interpretation of Statistics**

The descriptive statistics indicate that the Average Monthly Income (M = 4,243.97, SD = 2,116.64) is slightly higher than the Cost of Living (M = 3,705.13, SD = 1,982.22). Both variables show moderate variability, suggesting noticeable income and living cost differences across countries. The small skewness values (Income = 0.06; Cost = –0.04) and negative kurtosis values indicate that both distributions are approximately symmetrical and slightly flatter than the normal curve.

**3.3 Key Insights**

<img width="701" height="431" alt="Ảnh chụp Màn hình 2025-11-02 lúc 22 24 48" src="https://github.com/user-attachments/assets/1565c5d4-5ce0-4498-9aee-cbae7073c4ed" />

**Figure 1.** Comparison of Cost of Living and Average Income by Region

The chart compares total cost of living and income across regions, showing a proportional relationship between earnings and expenses.

**Insight 1 – Regional Comparison of Cost of Living and Average Income**

The bar chart shows that regions with higher average monthly income also tend to have higher living costs, particularly in Europe, North America, and Asia. However, the difference between income and cost of living remains positive in all regions, indicating that income generally exceeds expenses. This suggests a relatively balanced economic condition across regions, where higher wages compensate for higher living costs.

<img width="634" height="296" alt="Ảnh chụp Màn hình 2025-11-02 lúc 22 26 23" src="https://github.com/user-attachments/assets/629c04f0-66a6-4e67-8c94-f508fc17cddb" />

**Figure 2.** Relationship between Average Monthly Income and Cost of Living

The scatter plot shows that there is no strong linear relationship between income and living cost across countries.

**Insight 2 – Relationship between Average Monthly Income and Cost of Living**

The scatter plot reveals a very weak relationship between Average Monthly Income and Cost of Living across countries, as indicated by the nearly flat trendline. This means that nations with higher living costs do not consistently offer higher income levels, showing large variations in cost–income balance. The finding implies that purchasing power and economic well-being differ widely across regions, rather than following a uniform global pattern.

**3.4 Summary of Findings**

Overall, the descriptive statistics and visualisations suggest that although average income levels tend to exceed living costs globally, this relationship is not consistent across all regions.  
Economic variations and purchasing power differences contribute to unequal cost–income balances worldwide. These findings highlight the need to interpret income and cost-of-living data in a regional context rather than relying on global averages alone.






