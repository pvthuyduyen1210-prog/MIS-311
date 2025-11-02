# Part 1: Data Analysis and Insight

**##1. 	Data Overview**
The dataset, titled Cost of Living, was obtained from a global economic database that provides comparative statistics on living expenses and income levels across different regions. It contains **201 rows** and **5 columns**: Country, Year, Average_Monthly_Income, Cost of Living and Region.

Each record represents a country or territory with data collected for a specific year. The dataset aims to highlight variations in cost of living, income levels, and regional economic differences. The main purpose of this analysis is to explore whether higher living costs are associated with higher income levels and to identify global patterns across regions.

**##2. Data Cleaning**
The dataset was first cleaned to ensure accuracy and consistency before performing any statistical analysis.
Initially, Excel **TRIM(CLEAN)** formulas were applied to remove all unwanted white spaces and non-printable characters across the dataset, improving readability and preventing data entry inconsistencies.
Next, the dataset was examined for missing values using Excel’s **Filter** feature, with missing cells highlighted for review.
The inspection revealed two missing values in the **Average_Monthly_Income** column and two missing values in the **Region** column.
###To handle these missing values:
For Average_Monthly_Income, the mean substitution method was used.
The average income across all valid observations was calculated to be 4,243.97 USD, and this value was inserted in place of the two missing records.

For Region, a Pivot Table summarizing Region and Count of Region was created to identify the most frequent region.
The result showed that “North America” appeared most frequently, so this region was used to replace the two missing values.
Region	Count of Region
<img width="169" height="111" alt="Ảnh chụp Màn hình 2025-11-02 lúc 22 15 15" src="https://github.com/user-attachments/assets/9bf62278-8085-4bb3-91c1-4be142211dbd" />

Finally, the dataset was checked for duplicate rows, and two duplicates were identified and removed.
After cleaning, the dataset contained **199 complete** and unique rows, with no missing or duplicated data remaining.

**3. Descriptive Statistics**
**3.1 Overview of Descriptive Statistics**
Descriptive statistics were employed to explore the central tendencies, dispersion, and distribution of the dataset’s numerical variables. This step helps uncover underlying trends and prepares the foundation for generating meaningful insights.
		
<img width="483" height="243" alt="image" src="https://github.com/user-attachments/assets/065c4865-ebef-48e5-b2ed-0bf77bf82d02" />


