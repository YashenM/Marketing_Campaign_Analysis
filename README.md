# Marketing Campaign Analysis and Optimization

## Overview
This project analyzes customer data from iFood Brain Team’s marketing campaigns to evaluate their effectiveness and identify opportunities for optimization. The goal is to improve campaign targeting, increase response rates, and maximize revenue for the business. The analysis was conducted using **Excel**, with a focus on data cleaning, exploratory data analysis (EDA), and visualization.

## Dataset
The dataset used in this project is available on [Kaggle](https://www.kaggle.com/datasets/jackdaoud/marketing-data). It includes customer demographics, spending behavior, and campaign response data. Key features include:
- **Demographics**: Age, Education, Marital Status, Income.
- **Spending Behavior**: Amount spent on wines, meat products, fruits, etc.
- **Campaign Response**: Acceptance rates for 6 marketing campaigns.
- For a detailed description of the dataset features, see the [Data Dictionary](Data_Dictionary.md).

## Methodology
1. **Data Cleaning**:
   - Replaced missing values in the `Income` column with the average ($51,969).
   - Removed outliers in the `Year_Birth` column (e.g., 1893, 1899, 1900).
   - Corrected inconsistent `Marital_Status` values (e.g., "Alone" → "Single").
   - Deleted duplicate rows and rows with invalid data (e.g., "Absurd", "YOLO").

2. **Feature Engineering**:
   - Created new columns:
     - `TotalProducts`: Sum of spending on all product categories.
     - `TotalPurchases`: Sum of purchases across all channels.
     - `IncomeGroup`, `TotalProductsGrp`, `TotalPurchasesGrp`, `AgeGrp`: Segmented customers for analysis.

3. **Exploratory Data Analysis (EDA)**:
   - Analyzed spending behavior by income group, age group, marital status, and education level.
   - Evaluated campaign performance and response rates.
   - Visualized data using histograms, scatter plots, bar charts, and clustered column charts.

4. **Dashboard Creation**:
   - Built a dynamic Excel dashboard with interactive slicers for filtering data.
   - Included key visualizations such as:
     - Age and income distributions.
     - Campaign acceptance rates.
     - Relationships between spending, purchases, and customer demographics.

5. **Insights and Recommendations**:
   - Identified high-value customer segments (e.g., high-income, PhD holders).
   - Provided actionable recommendations for optimizing future campaigns.

## Results
### Key Findings
1. **High-Income Customers Drive Spending**:
   - Customers with incomes >$60k account for the majority of spending, particularly on wines ($349,532) and meat products ($188,655).
2. **Education Level Influences Engagement**:
   - PhD holders have the highest response rate (20.70%), followed by Master’s degree holders (15.45%).
3. **Campaign Performance**:
   - Campaign 4 has the highest acceptance rate (7.48%), followed by Campaign 3 (7.30%).
4. **Low Complaints Indicate High Satisfaction**:
   - Less than 1% of customers have complained, suggesting high satisfaction or low complaint reporting.

### Recommendations
1. **Target High-Value Segments**:
   - Focus on high-income customers (>$60k) and PhD holders for premium product campaigns.
2. **Optimize Purchase Channels**:
   - Enhance in-store and catalog experiences for high-income and married customers.
3. **Replicate Successful Campaigns**:
   - Analyze the strategies used in Campaigns 3 and 4 and apply them to future campaigns.
4. **Reduce Inefficiencies**:
   - Limit campaigns targeting low-income customers (<=$20k), as they have low response rates and spending.

### Impact
1. **Revenue Growth**:
   - Targeting high-income customers could increase wine and meat product sales by 10%, generating an estimated $50,000 in additional revenue annually.
2. **Cost Savings**:
   - Reducing campaigns for low-income customers could save $5,000 annually in marketing costs.
3. **Improved Engagement**:
   - Focusing on high-response segments (e.g., PhD holders, married customers) could increase campaign response rates by 15%.

## How to Use
1. **Open the Excel File**:
   - Download and open the `Marketing_Campaign_Analysis.xlsx` file.
2. **Navigate the Dashboard**:
   - Go to the **Dashboard** sheet for interactive visualizations.
   - Use slicers to filter data by income group, age group, or education level.
3. **Explore the Analysis**:
   - Check the **WorkingData** sheet for cleaned and processed data.
   - Review pivot tables and charts in other sheets for detailed analysis.

## Dependencies
- **Microsoft Excel**: The project uses Excel’s PivotTable, charting, and slicer functionality.
- **Excel Add-Ins**: None required.

## Author
Yashen Munasinghe  
yashen.munasinghe@gmail.com  
[LinkedIn Profile](http://www.linkedin.com/in/yashen-m)

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
