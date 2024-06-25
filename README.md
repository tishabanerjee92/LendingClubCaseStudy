
# Loan Default Prediction Analysis

## Project Overview
This project aims to analyze factors influencing loan default using Exploratory Data Analysis (EDA). The insights gained from the analysis will help in making decisions such as denying the loan, reducing the loan amount, or lending at a higher interest rate to risky applicants.

## Data Description
The dataset contains information about past loan applicants and their loan status, including whether they defaulted or not. It includes variables such as loan amount, interest rate, annual income, and more.

## Analysis Approach
1. **Data Loading and Understanding**: Initial examination of the dataset. We only included the following columns in our analysis: 'loan_amnt', 'funded_amnt', 'term', 'int_rate', 'installment', 'grade','sub_grade', 'emp_title', 'emp_length', 'home_ownership', 'annual_inc', 'verification_status', 'loan_status', 'dti', 'pub_rec', 'revol_bal', 'revol_util', 'total_acc' 
2. **Univariate Analysis**: We carried out univariate analysis of individual numeric and categorical columns using histogram, boxplots and bar charts.
3. **Bivariate Analysis**: Bivariate analysis of categorical vs numeric columns was done using boxplot. For categorical vs categorical columns we used bar charts on filtered data.
4. **Multivariate Analysis**: Multivariate analysis was carried out on numerical columns using heatmap.
5. **Derived Metrics**: Two additional columns were developed for further analysis - income group and loan amount category.
5. **Insights and Observations**: Key findings and recommendations were presented.

## Key Findings
1.	About 14% of the applicants defaulted in their loans.
2.	Income status of most of the borrowers who defaulted is unverified.
3.	Most of the loans are very low (5000 to 10000 dollars) and low (10000 to 15000 dollars) value loans.
4.	Interest rate levied on defaulters is significantly higher than that levied on borrowers who have fully paid their loans.
5.	Short term borrowers (36 months) defaulted more than long term borrowers (60 months). Short term loans are levied higher interest rates as compared to long term ones.
6.	Amongst top 10 employment types, employees of Bank of America default most followed by applicants of US Army
7.	Most of the borrowers belong to low and middle income group. Most of the borrowers who defaulted are also from the same income group.
8.	Median for debt-to-income ratio is near about 14 and most of the values are in between 7 to 19. This indicates that almost all of the borrowers have total monthly debt payments much higher than their self-declared monthly income. If this would have been true, then most of the borrowers would have defaulted in their payments but that is not the case. This might indicate borrowers have reported highly deflated monthly income figures.
9.	The above point is further supported by significant fraction of applicant's income being unverified. 45% of applicant's income is unverified. If we club unverified and source verified applicants together then we get about 70% applicants whose income is questionable. This very well resonates with the abnormally high debt-to-income ratio.
10.	There is wide variation in revol_bal values with the distribution being skewed towards lower values. This shows that most borrowers are not relying too much on credit. The average revolving credit utilization is 47%. The distribution of total accounts is a bit left screwed indicating that borrowers are not overly relying on credit. Most of the borrowers are having about 13 to 27 credit lines.


## Recommendations
- Refine loan approval criteria based on identified risk factors.
- Consider offering lower amounts or higher interest rates to risky applicants.
- Limit loans to borrowers whose income is unverified. Charge a greater interest rate for unverified borrowers
- Offer flexible payment plans for short term loans
- Include debt-to-income ratio as a factor for approving the loan and deciding the interest rates

## Files
- 'Ridhima_Banerjee.ipynb`: IPython Notebook containing the analysis.
- `Lending Club Case Study.pdf`: Presentation summarizing the analysis.
