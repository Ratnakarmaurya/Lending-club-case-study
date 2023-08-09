# Project Name: Lending Club Case Study

## Table of Contents

- [General Info](#general-information)
- [Technologies Used](#technologies-used)
- [Observations](#observations)
- [Conclusions](#conclusions)
- [Acknowledgements](#acknowledgements)

## General Information

### Project Information

> The project is a data science project that uses the lending club data set to predict whether a loan will be defaulted or not.

### Project Background

> This firm stands as the leading digital loan marketplace, facilitating a range of loans including personal, business, and medical financing. Borrowers can effortlessly obtain loans with reduced interest rates through a rapid online platform. Similar to the majority of lending enterprises, extending loans to ‘high-risk’ applicants constitutes the most significant origin of financial shortfall, denoted as credit loss. This signifies the monetary value that the lender loses when the borrower declines payment or absconds with the borrowed funds. In simpler terms, borrowers who fail to meet their obligations contribute the most to the lenders' financial setbacks. In this particular situation, individuals categorized as 'charged-off' are synonymous with 'defaulters'. 

### Project Statement

> Find the driving factors which lead to the defaulted loans which are major source of loss for the company.

### Data Set

> The data set is a csv file with the loan data for the Lending Club.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Observations
### Univariate Analysis
 - The count of defaulted loans is around one-seventh of the count of fully paid loans.
 - Most loans have a term of 36 months, with fewer loans having a term of 60 months.
 - Interest rates exhibit a peak in the 5-10 and 10-15 ranges, with a dip around 10.
 - A significant portion of loans fall under grades 'A' and 'B', signifying a prevalence of high-grade loans.
 - The majority of borrowers possess over 10 years of work experience.
 - Most borrowers are either on mortgage or rent, with limited property ownership.
 - About half of the borrowers are verified by the company or have a source of verification.
 - Annual income follows a left-skewed normal distribution, indicating a predominant occurrence of low annual incomes.
 - Debt consolidation accounts for the largest proportion of loan purposes, followed by credit card financing.
 - Borrowers primarily originate from major urban centers such as California, New York, Texas, Florida, etc.
 - A significant number of borrowers have a high debt-to-income ratio (DTI), mainly falling within the 10-15 range.
 - Public Recorded Bankruptcy is infrequent among the borrowers.
 - Loan issuance is concentrated in the final quarter of the year.
 - Loan approvals exhibit an exponential increase over time, suggesting an upward trend in the approval rate.
### Segmented Univariate Analysis
- Debt consolidation emerges as the most common loan purpose, showing the highest counts for both fully paid and defaulted loans.
- The mean and 25th percentile are identical between fully paid and defaulted loans. However, defaulted loans display a larger 75th percentile, indicating a higher occurrence of larger loan amounts facing default.
- The likelihood of default is higher for loans with a 60-month term compared to those with a 36-month term. Conversely, the 36-month term demonstrates a higher likelihood of being fully paid.
- Grade distribution varies with loan terms: 36-month loans are predominantly grades A and B, while 60-month loans include a mix of grades B, C, and D.
- Loan status corresponds with DTI ratio, showing higher counts of defaulted loans in the 10-15 DTI range, although higher DTI ratios are more prone to default.
- Defaulted loans are less common among borrowers who own property compared to those on mortgage or rent.
- Borrowers with annual incomes under dollar 50,000 are more inclined to default, while those with higher incomes are less likely to default.
- Fully paid loans demonstrate an exponential rise over time, contrasting with defaulted loans.
- Defaulted loan amounts rise with interest rates, with a decline beyond 17.5% interest.
- Borrowers with over 10 years of experience are more likely to default but also have an increased chance of fully repaying the loan.
### Bivariate Analysis
- Risk increases with grade, leading to higher interest rates.
- Grade A, indicating lower risk, corresponds to lower DTI ratios, implying that higher-grade loans exhibit lower default rates.
- Borrowers with no history of Public Recorded Bankruptcy are perceived as safer candidates for loan issuance.
- Recommendations
- Key Predictive Factors for Default Risk Mitigation and Credit Loss Avoidance:
- Debt-to-Income Ratio (DTI)
- Loan Grades
- Verification Status
- Annual Income
- Public Recorded Bankruptcies
- Additional Considerations for Identifying 'Default' Candidates:
- Borrowers from non-major urban cities (not California, New York, Texas, Florida, etc.)
- Borrowers with annual incomes in the $50,000 to $100,000 range.
- Borrowers with a history of Public Recorded Bankruptcy.
- Borrowers assigned lower grades (E, F, G) indicating higher risk.
- Borrowers with significantly high Debt-to-Income ratios.
- Borrowers with over 10 years of work experience.
## Conclusions

- Major Driving factor which can be used to predict the chance of defaulting and avoiding Credit Loss:
  1. DTI
  2. Grades
  3. Verification Status
  4. Annual income
  5. Pub_rec_bankruptcies
- Other considerations for 'defaults' :
  1. Burrowers from large urban cities like california, new york, texas, florida etc.
  2. Burrowers having annual income in the range 50000-100000.
  3. Burrowers having Public Recorded Bankruptcy.
  4. Burrowers with least grades like E,F,G which indicates high risk.
  5. Burrowers with very high Debt to Income value.
  6. Burrowers with working experience 10+ years.


## Technologies Used

- Pandas==version 1.3.4
- NumPy==version 1.20.3
- Seaborn==version 0.11.2
- MatplotLib== version 3.4.3
- Plotly== 5.7.0
- openpyxl==3.1.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

This project is case study for the Machine Learning and Artificial Intelligence course from IIITB

Made by @ratnakarmaurya
Made by @meghnamajumder

