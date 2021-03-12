# Loan Data from Prosper
## by Marc Campmany


## Dataset

> - In this project the main goal has been to analyze the features related mainly to the _Borrower's APR_ (annual interest rate charged). The variables studied have been the _Original Loan Amount, Borrower's Prosper Rating, Loan Term, Borrower's Income Range, Employment Status, Occupation and aim of the loan_.
> - The original data set ('prosperLoanData.csv') contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. After cleaning operations, the dataset studied contains 83.968 unique loans with 15 related features ('LoanData_cleaned.csv')


## Initial hypothesis
> - I expect that the LoanOriginalAmount will have a negative effect on the APR of the loan: the larger the total loan amount, the lower the APR.
> - I also think that the borrowers stated Income Range, loan term, Debt to Income and employment status will also have effects on the APR and the Rating associated with the borrower.
> - I think that Loan Amounts and their Listing Category vs IncomeRange / terms / Ratings will be related

## Findings
> - The distribution of the borrowers APR is spiked on 0.36 which is the typical rate applied to small dollar lending Loans [https://qcashfinancial.com/36-percent-apr-for-small-dollar-loans/]
> - The majority of loan Terms are 36 months, the year with higher Loan requests was 2013, the risk scale distribution for the Loans of this analysis follows a Normal distribution with C-rated Loans as the mean.
> - The great majority of borrowers are employed and have a debt to income ratio of 1:4.

> - The borrower APR is negatively associated with the loan original amount, which means that the higher the loan amount, the lower the APR.
> - The Prosper Rating also has a strong effect on the borrower APR, which decreases with the better rating as shown in the boxplots.
> - We can see that the Loans with more Terms and the best ranked (AA) are the ones that are charged a lower interest rate (APR). Also when the borrower is employed/full-time the APR is also lower. Regarding the IncomeRange is easy to see that the higher the income range of the borrower, the lower the APR.
> - Loan Amounts show that are related to terms because higher loans require higher terms. We can also observe that, understandably, borrowers with higher incomes or employed (variables= employed, self-employed, full-time) acquire higher Loans.

> - The multivariate exploration of the _Borrower's APR_ vs _Original Loan Amount_ and adding _Prosper's Rating_ showed that the relationship between _Borrower APR_ and _Loan Amount_ goes from negative on ratings HR-B to slighly positive relationship on ratings A and AA.
> - We can also see that the better the _Prosper Rating_ the less _Interest Rate_ (APR) is charged. And analyzing together with the _Loan Terms_ we can see that, as the Loan _Rating_ gets better, the pattern is that the _Terms_ increase. This is probably also due to the increase of the _Loan Amount_.
