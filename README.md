# HADS-Housing-Affordability
- All files are self-contained analysis reports that include necessary variables. 

- Many businesses still use Excel as a primary "database"/data storage device; to accomodate this, all files are Excel based and analysis was run using Excel. 

-Market value was measured across various years to determine if there was a difference between occupied and unoccupied housing units.

## Processing Instructions:
- Use Excel or application that can open .xlsx files to view the analysis report. 
- Each worksheet is labeled to include "Summary Report", "Descriptive Statistics", "Graphs", and "Test".

## Steps to Transformation:
### Data was tidied by: 
- All data points for VALUE variable less than $1000.00 were removed per project instructions.
- All NULL values were removed. Missing values were missing because the original data source has odd-numbered years in 1985-2009 and "selected only records representing completed interviews for occupied and vacant units, excluding usual residence elsewhere (URE) and noninterview records." per HADS documentation file. https://www.huduser.gov/portal/datasets/hads/HADS_doc.pdf

1. Dataset was downloaded from host website: https://www.huduser.gov/portal/datasets/hads/hads.html
2. VALUE and STATUS variable were used for analysis.
   - VALUE is numeric continuous, normally distributed. STATUS is categorical, nominal consisting of two independent groups of "occupied" and "vacant".
3. VALUE was determined to be the dependent variable, STATUS was determined to be the independent variable.
4. VALUE was grouped into categories "unoccupied" and "vacant", reflecting the STATUS of each unit.
5. Worksheets were created to hold four categories for the analysis: 
   - Summary Report identifies and answers the business question/what was measured
   - Descriptive Statistics identifies and calculates descriptive statistics
   - Graphs displays histograms and boxplots
   - Tests holds results for statistical tests
6. Hypothesis tested: "is there a difference between the market VALUE for "occupied" and "vacant" STATUS housing units across various years?" A two-tailed t-Test assuming unequal variances was run to determine statisical significance between group means; results are listed in the "Summary Report" worksheet.

