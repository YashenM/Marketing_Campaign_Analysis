# Marketing Campaign Analysis and Optimization

## Overview
This project analyzes customer data from iFood Brain Team’s marketing campaigns to evaluate their effectiveness and identify opportunities for optimization. The goal is to improve campaign targeting, increase response rates, and maximize revenue for the business. The analysis was conducted using **Excel**, with a focus on data cleaning, exploratory data analysis (EDA), and visualization.

## Dataset
The dataset used in this project is available on [Kaggle](https://www.kaggle.com/datasets/jackdaoud/marketing-data). It includes customer demographics, spending behavior, and campaign response data. Key features include:
- **Demographics**: Age, Education, Marital Status, Income.
- **Spending Behavior**: Amount spent on wines, meat products, fruits, etc.
- **Campaign Response**: Acceptance rates for 6 marketing campaigns.

For a detailed description of the dataset features, see the [Data Dictionary](Data_Dictionary.md).

## Repository Structure
Here’s an overview of the files and folders in this repository:

```
Marketing_Campaign_Analysis/
├── README.md               # Overview of the project
├── Executive_Summary.pdf   # Concise report of findings and recommendations (to be added)
├── Data_Dictionary.md      # Description of dataset features
├── LICENSE                 # Terms of use for the project
├── Data/                   # Folder containing raw data
│   └── marketing_data_raw.csv  # Original dataset
├── Analysis/               # Folder containing analysis files
│   └── Marketing_Campaign_Analysis.xlsx  # Excel file with cleaned data, analysis, and dashboard
└── Screenshots/            # Folder containing dashboard and chart images
    └── Dashboard.png       # Screenshot of the Excel dashboard
```

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
   - Customers with incomes >$60k account for the majority of spending and thus contribute the majority of the business revenue.
2. **Revenue Contribution by Product**:
   - Wines ($678,683) and meat products ($372,668) make up 78% of the total revenue.
3. **Education Level Influences Engagement**:
   - PhD holders have the highest response rate (20.70%), followed by Master’s degree holders (15.45%).
   - The majority of customers are graduates (1,126), followed by PhD holders (483), but graduates’ response rate is relatively low (13.41%).
4. **Campaign Performance**:
   - The final campaign has the highest acceptance rate (14.78%), followed by Campaign 4 (7.48%).
5. **Low Complaints Indicate High Satisfaction**:
   - Less than 1% of customers have complained during the last two years, suggesting high satisfaction or low complaint reporting.
  
### Recommendations
1. **Target High-Value Segments**:
   - Focus on high-income customers (>$60k) and PhD holders for premium product campaigns.
   - Promotions should focus on graduates aggresively.
   - Focus campaigns on fish products, sweet products, gold products, and fruit more aggressively, as data suggests these categories combined contribute up to 22% of the total revenue.
2. **Optimize Purchase Channels**:
   - Enhance in-store and catalog experiences for high-income and married customers.
3. **Replicate Successful Campaigns**:
   - Analyze the strategies used in final campaign and campaign 4, and apply them to future campaigns.
4. **Reduce Inefficiencies**:
   - Limit campaigns targeting low-income customers (<40k), as they have low response rates and spending.

### Impact
1. **Revenue Growth**:
   - Targeting graduate customers and improving their engagement by 10% could result in an estimated $70k in additional annual revenue.
   - A 10% increase in the sales of fish products, sweet products, gold products, and fruit could generate more than $30k in additional revenue.
2. **Cost Savings**:
   - Reducing campaigns for low-income customers could save more than 30% annually in marketing costs.
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
