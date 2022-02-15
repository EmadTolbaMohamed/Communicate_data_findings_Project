# Communicate_data_findings_Project
Project for Advanced Data Analysis Udacity Nano Degree

## Exploration of Loan Dataset from Prosper
### Dataset Overview
The dataset has 113937 rows of loans entries and 81 features(columns). Each loan contain information on the borrowered's background information and details regarding the loans. We selecting only 10 features(columns) for investegation and after dropping Null values the data will contains 84853 loans entries.

### Summary of Findings
This project will investigate what factors affect a loan’s outcome status?

#### From Univariate Exploration
Loan Status variable has very large number of Current loans which was excluded. After excluding the loans with status Current, there are 69.54% loans with status 'Completed', 3.55% with status 'Defaulted', 8.03% with status 'PastDue' and 18.87% with status 'Chargedoff'. So we will filter LoanStatus with the Completed and Defaulted status to investigate what factors affect a loan’s outcome status?

- The distribution of Stated Monthly Income is severe right skewed due to the outliers which are presented with the high incomes. The most Monthly Income is between 0 and 20000 so we will filtered them.
- The distribution of AvailableBankcardCredit is severe right skewed due to the outliers which are presented with the high AvailableBankcardCredit.
- Most loans are 36 month terms followed by 60 month and the least is 12 month
#### From Bivariate Exploration
- the mean of Stated Monthly Income for LoanStatus with the Completed status is slightly higher than that one the Defaulted status. I.e higher Monthly Income loan takers are more likely to be Completed.
- the mean of Borrower APR for LoanStatus with the Defaulted is higher than that one the Completed status.
- ProsperScore '1' has the highest number of Defaulted cases and ProsperScore '10' has the least number of Defaulted cases as expected large score being least risky.

- Loans with lower Prosper Score have higher Borrower APR.

- There are negative correlation between CreditScoreRangeUpper and BorrowerAPR.
- There are moderate negative correlation between LoanOriginalAmount and BorrowerAPR.
#### From Multivariate Exploration
- Most Defaulted LoanStatus are in long Term Loans with 36 months terms followed by 60 months .
- Almost all loans with Trem of 12 months are Completed Status. No strong positive correlation are present between features. All correlation present are weak to mederate.
### Key Insights for Presentation
- Loan Status variable has very large number of Current loans which was excluded. After excluding the loans with status Current, there are 69.54% loans with status 'Completed', 3.55% with status 'Defaulted', 8.03% with status 'PastDue' and 18.87% with status 'Chargedoff'.

- Borrower’s Annual Percentage Rate (APR) is normal distribution with exceptional high count at BorrowerAPR about 0.36 %.

- The mean of Borrower APR for Defaulted LoanStatus is higher than that one the Completed status.

- ProsperScore '1' has the highest number of Defaulted cases and ProsperScore '10' has the least number of Defaulted cases as expected large score being least risky.
