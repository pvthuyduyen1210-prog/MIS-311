# Part 1: Data Analysis and Insight

**1. Data Overview**

**Dataset Description:**
The dataset titled “Cost of Living” provides historical economic data on average monthly income and cost of living across 12 countries from 2000 to 2023. It serves as a valuable resource for analyzing global economic trends, affordability, purchasing power, and regional differences in living standards.


<img width="426" height="497" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 34 03" src="https://github.com/user-attachments/assets/b6d014dd-a48d-4c97-bf9d-4560f43aace4" />




Although the exact data source is not explicitly stated in the file, it likely consolidates information from reputable international databases, including:

+ Numbeo (crowdsourced cost-of-living indices)

+ World Bank (income and poverty metrics)

+ International Labour Organization (ILO) (wage and employment data)

+ International Monetary Fund (IMF)  macroeconomic indicators

+ National statistical offices of each country

**Structure of the Data:**

**Sheet name**: 01_Cost of Living

**Number of rows:** 201

**Number of columns:** 5

**Column names:**

+ Country: Name of the country.

+ Year: The year of observation.

+ Average_Monthly_Income: Average monthly income per person in local or standardized currency.

+ Cost_of_Living: An index or value representing the average cost of living in that country.

+ Region: The geographical region the country belongs to (e.g., Europe, Asia, Africa).

**Context and Potential Analysis:**

This dataset can be used to explore economic disparities, compare income versus cost of living across regions, or identify trends in living affordability over time. It is suitable for both descriptive and inferential statistical analysis. For example, investigating whether higher income levels correlate with higher costs of living globally.

**2. Data Cleaning**

The dataset was first cleaned to ensure accuracy and consistency before performing any statistical analysis.
The dataset was carefully examined for missing values using Excel’s Filter feature, with blank cells highlighted for manual inspection.

<img width="604" height="94" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 38 26" src="https://github.com/user-attachments/assets/2174d92b-3d90-4f92-bdf1-1dcafb05731f" />

During this process, four missing entries were identified:
Two missing values in the column Average_Monthly_Income (Column C) at rows 160 and 176, where income data was not recorded.

<img width="475" height="48" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 51 22" src="https://github.com/user-attachments/assets/0a545fe6-c365-4d82-8ce5-33c6a6203585" />

Two additional missing values in the column Region (Column E) at rows 26 and 39, indicating the absence of regional classification for those countries.

<img width="606" height="74" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 39 37" src="https://github.com/user-attachments/assets/2b1950fa-6c13-45fe-9322-056fe7eb9ee4" />

These missing values were documented for further handling to ensure data completeness and analytical accuracy.

**To handle these missing values:**

+ For the two missing values in the **Average_Monthly_Income** column (Rows 160 and 176), the Median imputation method was applied. This technique replaces missing data with the median value of the column, in this case, 4,266.66 ensuring that the filled values represent the central tendency of the dataset without being affected by extreme outliers.

  
<img width="605" height="94" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 40 41" src="https://github.com/user-attachments/assets/0fa1fb60-634e-46d2-bf01-63c97be23229" />

This method was chosen because it helps maintain data integrity and consistency, while avoiding the loss of valuable records through deletion. As a result, the dataset remains both complete and representative, supporting more reliable statistical analysis.

<img width="601" height="41" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 41 37" src="https://github.com/user-attachments/assets/0860af26-b4d8-4fa6-88f2-3a5f8d31e2a9" />

<img width="605" height="43" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 41 53" src="https://github.com/user-attachments/assets/e069f9ad-c589-4ebb-b195-d4d8ed7eb507" />

For the two missing values in the Region column (Rows 26 and 39), I used an imputation manual that showed that both rows corresponded to Mexico. 

<img width="605" height="40" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 42 34" src="https://github.com/user-attachments/assets/4c8ce755-7902-4d68-84a3-c06200af6742" />

Since another record for Mexico (Row 42) already listed the region as North America, these missing values were filled accordingly. This approach ensures data consistency and accuracy by using existing information within the dataset instead of external.

<img width="614" height="37" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 43 03" src="https://github.com/user-attachments/assets/5121dc10-bed7-4057-96ff-90763634c83b" />

<img width="559" height="34" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 43 21" src="https://github.com/user-attachments/assets/971cd28d-41ba-4aaf-b2c1-205ce1d36c0a" />

Finally, the dataset was checked for duplicate rows, and two duplicates were identified and removed.

<img width="205" height="172" alt="Ảnh chụp Màn hình 2025-11-05 lúc 13 43 50" src="https://github.com/user-attachments/assets/06c21668-fe97-4c0d-af4e-874a098bb3e5" />

After cleaning, the dataset contained 199 complete and unique rows, with no missing or duplicated data remaining.


**3. Descriptive Statistics**
   
**3.1 Overview of Descriptive Statistics**

Descriptive statistics were employed to explore the central tendencies, dispersion, and distribution of the dataset’s numerical variables. This step helps uncover underlying trends and prepares the foundation for generating meaningful insights.
		

<img width="886" height="443" alt="Ảnh chụp Màn hình 2025-11-02 lúc 22 21 48" src="https://github.com/user-attachments/assets/452eb1fb-274b-450e-a86b-c49cb85ac6ea" />

Table 2. Descriptive Statistics Summary

**3.2 Interpretation of Statistics**

The dataset reveals that the average monthly income (4,244 USD) is only slightly higher than the average cost of living (3,705 USD). This small gap suggests that in many countries, people are living close to the financial edge, with limited room for savings or discretionary spending. It reflects a common global pattern, wages may rise over time, but living costs tend to increase at a similar pace.

The standard deviation values (≈ 2,117 for income and ≈ 1,982 for cost of living) show noticeable variation between countries. High-income economies such as the United States or Germany enjoy stronger purchasing power, while developing countries like India or South Africa face much lower incomes but also reduced living costs. This highlights the economic diversity and the unequal distribution of prosperity worldwide.

Meanwhile, skewness values near zero indicate that both variables are fairly symmetrical, meaning no country group dominates the dataset with extremely high or low figures. The negative kurtosis values suggest a flatter distribution, implying that most nations fall around the global average rather than at the extremes.

Overall, the statistics portray a balanced but strained global economy, where higher income often comes hand-in-hand with higher living expenses. The data paints a realistic picture of how affordability and purchasing power remain ongoing challenges, even as economies grow.


**3.3 Key Insights**

<img width="701" height="431" alt="Ảnh chụp Màn hình 2025-11-02 lúc 22 24 48" src="https://github.com/user-attachments/assets/1565c5d4-5ce0-4498-9aee-cbae7073c4ed" />

**Figure 1.** Comparison of Cost of Living and Average Income by Region

The chart compares total cost of living and income across regions, showing a proportional relationship between earnings and expenses.

**Key Insight 1: Regional Income - Cost Gap Reflects Economic Balance and Living Standards**

The comparison between Average Monthly Income and Cost of Living by region reveals a striking pattern: while income levels generally exceed living costs in all regions, the margin varies significantly.

Regions like Asia and Europe show the highest total income and cost of living, suggesting strong economies but also high lifestyle expenses, North America has a more balanced relationship, where high incomes are matched by equally high living costs. In contrast, Africa and South America exhibit much lower income and cost values, reflecting more affordable living but limited purchasing power.

This insight would be especially relevant for policy makers, economic planners, and multinational companies seeking to understand regional economic conditions. 

+ For governments, it highlights the need to balance wage growth with cost-of-living increases to protect citizens’ real purchasing power. 

+ For businesses, it provides strategic guidance on setting fair wages, pricing products, or expanding into regions with more sustainable affordability ratios.

Ultimately, this visualization underscores a fundamental truth: higher income does not always translate to better living standards. The cost of living rises in parallel, meaning real financial comfort depends not only on earnings but also on how much those earnings can actually buy in each region.


<img width="634" height="296" alt="Ảnh chụp Màn hình 2025-11-02 lúc 22 26 23" src="https://github.com/user-attachments/assets/629c04f0-66a6-4e67-8c94-f508fc17cddb" />

**Figure 2.** Relationship between Average Monthly Income and Cost of Living

The scatter plot shows that there is no strong linear relationship between income and living cost across countries.

**Key Insight 2: Higher Income Does Not Necessarily Translate to Better Living Standards**

The scatter plot illustrating the relationship between Average Monthly Income and Cost of Living reveals a notable finding, the regression line is almost flat, indicating a weak or negligible correlation between the two variables. In other words, earning more does not automatically mean living better or having lower financial pressure.

This insight is particularly valuable for policy makers, economists, and international businesses.

+ For governments, this finding serves as a warning: increasing nominal wages alone may not improve people’s real quality of life if living expenses rise at a similar or faster rate. Effective policies should therefore aim to control inflation and stabilize essential costs to protect citizens’ purchasing power.
  
+ For businesses, this insight suggests that high-income markets are not always high-potential markets because consumers’ disposable income might still be limited once basic living costs are covered.
  
+ From an economic perspective, the weak correlation highlights a disconnect between nominal income growth and real income stability, a pattern increasingly observed worldwide. It underscores that while salaries may appear higher on paper, real purchasing power often remains stagnant due to rising living costs.

In essence, this chart tells a simple but powerful story: a higher paycheck does not guarantee a higher standard of living. Sustainable economic growth should therefore focus on enhancing real income, ensuring that people not only earn more but can truly afford a better life. 

** Summary of Findings**

The analysis shows that while income generally rises with the cost of living, the balance between the two differs across regions. The weak correlation between income and living costs suggests that earning more does not always mean living better. True economic progress requires both sustainable income growth and effective control of living costs to improve real quality of life.







