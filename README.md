# ADIDAS SALE FORECASTING
*To remain competitive in the US market, Adidas wants to use historical US sales data to obtain valuable insights into the company's performance, market segmentation and sales trend, and use these insights to drive informed decision-making, help optimize strategies, and achieve its sales and business objectives.*

### 1. Data
The selected dataset for this project is Adidas 2020-2021 US sales data, available at https://data.world/stellabigail/adidas-us-sales-datasets.  This dataset, in Excel format, and with a size of 682.28 KB, comprises 9,648 rows and 13 columns.

### 2. Data Wrangling
The dataset is relatively straightforward and doesn’t contain any missing data.  I spent most of my data wrangling time addressing the below issues:
- #### Data Format:
  Initially, all columns in the dataset were categorized as 'object' data types. To ensure precise and uniform data representation, I adjusted the data type of each column based upon the inherent characteristics of each column and its intended utilization in the model.
- #### Data Integrity:
   1) Four rows were identified with 0 units sold, 0 total sales, and 0 operating profit, yet displaying a non-zero operating margin. Since the main focus of our analysis centers around total sales and operating profit, and the inconsistent non-zero operating margin values would not adversely impact the results, I opted to retain these four rows.
   2) When using the formula "Price per Unit x Units Sold = Total Sales" to validate the accuracy of the "Total Sales" values, I found a total of 3886 rows with a mismatch between the calculated and original Total Sales values.  In a real business environment, we’ll need to acquire additional sales data or order details to conduct further analysis.  However, for this project, due to the lack of supplemental data, I proceeded with the assumption that all three original data columns were accurately recorded, and the disparity between calculated and original Total Sales values was caused by factors beyond my understanding.
   3) To validate the accuracy of the "Operating Margin" values, I calculated the operating margin for each entry using the formula "Operating Profit / Total Sales = Operating Margin", and compared the calculated values with the original numbers in the dataset. A total of 848 rows with a mismatch were found.  Upon a closer look, I concluded that the miscrepancies between the calculated values and the original values are so minor that they could be ignored.
 
### 3. EDA
I plotted a timeline chart using aggregated monthly sales volume to show that Adidas US sales have been consistently increasing from 2020 to 2021, suggesting a positive upward trend.
Based upon boxplots on the 

