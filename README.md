# HADS-Housing-Affordability
All files are self-contained analysis reports that include necessary variables. 

Many businesses still use Excel as a primary "database"/data storage device; to accomodate this, all files are Excel based and analysis was run using Excel. 

## Processing Instructions:
- Use Excel or application that can open .xlsx files to view the analysis report. 
- Each worksheet is labeled to include "Summary Report", "Descriptive Statistics", "Graphs", and "Test".

## Steps to Transformation:
### Data was tidied by: 
- All data points for VALUE variable less than $1000.00 were removed.
- All NULL values were removed.

1. Dataset was downloaded from host website: https://www.huduser.gov/portal/datasets/hads/hads.html
2. VALUE and STATUS variable were used for analysis.
3. VALUE was determined to be the dependent variable, STATUS was determined to be the independent variable.
4. VALUE variable was grouped into categories "unoccupied" and "vacant", reflecting the STATUS of each unit.
5. Worksheets were created to hold four categories for the analysis: 
   - Summary Report identifies and answers the business question.
   - Descriptive Statistics identifies and calculates descriptive statistics
   - Graphs displays histograms and boxplots
   - Test holds results for statistical tests run
10. VALUE is numeric continuous, normally distributed. STATUS is nominal, categorical consisting of two independent groups of "occupied" and "vacant".
11. Hypothesis tested was if there is a difference between the market VALUE for "occupied" and "vacant" STATUS. A two sample t-Test assuming unequal variances was run to determine statisical significance between group means; results are listed in the "Summary Report" worksheet.

