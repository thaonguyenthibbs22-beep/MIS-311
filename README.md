
# I. Data Overview

The **"US Baby Names"** dataset is a comprehensive historical record of newborn naming trends in the United States over a century (from 1880 to 2024).

With a total of four primary columns **(4 distinct variables)** and **30,001 rows**, this dataset integrates categorical dimensions (Name, Sex) with quantitative and time-series data (Year, Count) enabling to forecast future demographic shifts and understand the mathematical distribution of name popularity across nearly 150 years.
|Variables| Variable Description|
|---------|---------------------|
|Year|Year of birth (1880–2024)|
|Name| First name|
|Sex| F (Female) or M (Male)|
|Count|Number of babies given that name in that year|
# II. Data Cleaning
***1. Mising Values***

I utilized **Excel’s Go To Special (Blanks)** feature to perform a comprehensive scan for missing values across all variables. The results confirmed that there are no null values in the Year, Name, Sex, or Count columns.

<img width="1917" height="720" alt="Ảnh chụp màn hình 2026-05-17 211443" src="https://github.com/user-attachments/assets/43ae1813-da77-478a-8a52-32605a024db1" />
<img width="1912" height="764" alt="Ảnh chụp màn hình 2026-05-17 211457" src="https://github.com/user-attachments/assets/b7ca5c7e-ac63-47b4-a6b5-73467907b271" />


***2. Remove Duplicates***

To maintain data integrity, I performed a **Remove Duplicates** operation by selecting all four attributes: Year, Name, Sex, and Count. This ensures that only identical records across all dimensions were removed, while legitimate recurring names in different years or gender categories were preserved for analysis.

<img width="1909" height="725" alt="Ảnh chụp màn hình 2026-05-17 212823" src="https://github.com/user-attachments/assets/b4f5635d-cdca-4e28-a7b9-750a410b0f90" />

**=>Overall, the data is highly consistent with no missing or duplicate entries found, providing a clean and reliable foundation for exploring historical naming trends in the US.**

# III. Descriptive Statistics
***Genaral Overview***

"The data reveals an extremely large disparity in naming trends. While half of the names on the list are for children of 12 or fewer (Median = 12), the average is 157, accompanied by a very high standard deviation (1162). This demonstrates that the naming market is dominated by a few 'hit' names with a total of over 81,000 children, while the vast majority of the remaining names are very rare."

<img width="233" height="364" alt="Ảnh chụp màn hình 2026-05-17 220407" src="https://github.com/user-attachments/assets/d3ac0d3d-2f15-4c19-ac0e-73b5075a0b7a" />



***1. Insight 1***

The analysis of the Top 10 names reveals a massive concentration of popularity, led by David with over 92,500 total births. A deep dive into the temporal data shows that this dominance is driven by a historic peak in 1956, where the name David alone accounted for 81,650 births—nearly 88% of its total across all years.

This highlights that naming trends in the US are not just gradual shifts but are often characterized by sudden cultural explosions, where a single name can dominate the national landscape for a specific period before returning to a baseline level.

<img width="1118" height="581" alt="Ảnh chụp màn hình 2026-05-17 223324" src="https://github.com/user-attachments/assets/a73ecba8-af8e-43c3-86de-e6ff0c8b4143" />

***2. Insight 2***

The visualization highlights a significant behavioral gap: while the female population (F) shows a high variety of unique names (17,842), the male population (M) is more concentrated within a smaller pool of 12,158 names.

This indicates that naming girls is driven by a desire for uniqueness and individuality, whereas naming boys leans toward traditional and recurring classics, as reflected by the higher 'Average per Name' for males (181.6 vs 140.8).

<img width="868" height="534" alt="Ảnh chụp màn hình 2026-05-17 230141" src="https://github.com/user-attachments/assets/e2068d09-7e52-4627-8371-da52fb3f0c20" />
