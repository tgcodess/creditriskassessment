dataset link : https://www.kaggle.com/datasets/devanshi23/loan-data-2007-2014
## Credit Risk Assessment Project: An Overview

## Project Title: Comprehensive Credit Risk Assessment Using Data Analytics

## Objective: To develop an advanced credit risk assessment model for evaluating the likelihood of loan defaults. 

## Project Description:

In this project, I conducted a thorough analysis of loan performance metrics to assess credit risk. The project involved:

## Data Preparation and Analysis:

## Data Collection: Utilized a dataset from financial institutions, capturing various loan-related attributes such as loan_status, loan_amount, interest_rate, and payment_time.
## Data Cleaning and Aggregation: Aggregated data to calculate key performance indicators such as the total number of customers and their corresponding loan statuses. Calculated the percentage of customers in each category to understand the distribution of loan statuses.
# Credit Risk Analysis:

## Loan Status Distribution: Analyzed the distribution of loan statuses (Good Loan, Bad Loan) to identify trends and anomalies.
## Bad Loan Rate Analysis: Assessed the rate of bad loans based on different loan attributes:
## Loan Amount: Evaluated how varying loan amounts influence the likelihood of a loan becoming a bad loan. This analysis involved grouping data by score_group, loan_status, and loan_amount, calculating the proportion of bad loans within each category, and visualizing these insights using bar plots.
## Interest Rate: Investigated the correlation between interest rates and the rate of bad loans. The analysis was conducted by grouping data by score_group, loan_status, and interest_rate, followed by calculating and visualizing bad loan rates for different interest rate brackets.
## Payment Time: Explored the impact of payment time on loan default rates. Grouped data by score_group, loan_status, and payment_time to determine the bad loan rate across different payment time categories.
## Visualization and Interpretation:

Created detailed visualizations to illustrate the bad loan rates across different variables. Plots included bar charts highlighting the risk levels associated with different loan amounts, interest rates, and payment times.
Incorporated vertical lines and annotations to mark critical thresholds and provide clear visual cues for risky loan categories.
## Insights and Recommendations:

Identified that customers with low credit scores and high loan amounts or high interest rates are more likely to default.
Recommended focusing on these high-risk segments for closer scrutiny and risk management.
Suggested integrating this risk assessment model into existing credit evaluation frameworks to enhance decision-making processes and minimize financial risk.

## Technical Details

Programming Language: Python
Libraries Used: Pandas, Matplotlib, Seaborn, NumPy
Key Modules:
d_frame(): Function to aggregate and calculate loan status distributions.
plot(): Function to generate bar plots for loan status categories.
df_bad_loan(): Function to compute bad loan rates based on specified criteria.
plot_bad_loan(): Function to visualize bad loan rates across various attributes.
Usage

## Data Preparation: Load and preprocess the dataset to prepare for analysis.
## Credit Risk Analysis: Utilize the provided functions to analyze loan statuses and compute bad loan rates based on different criteria.
## Visualization: Generate visualizations to interpret the results and identify high-risk areas.
## Insights: Review the analysis and insights to make informed decisions on credit risk management.

## Financial Terms and Methodology
Credit Risk Assessment: We utilize statistical and analytical methods to evaluate the risk that borrowers will default on their loans. This assessment helps in identifying high-risk loans and improving risk management strategies.

Loan Status: Loans are categorized as either 'Good Loan' or 'Bad Loan.' The project analyzes these classifications to determine the proportion of bad loans within the dataset.

Bad Loan Rate: The percentage of loans classified as 'Bad Loan' is calculated and analyzed to gauge the overall risk associated with different loan amounts, interest rates, and payment times.

Loan Amount: The impact of loan sizes on credit risk is examined. We analyze how different loan amounts correlate with the likelihood of loan defaults.

Interest Rate: The project's analysis includes evaluating how varying interest rates affect the bad loan rate. Higher interest rates may increase default risk if borrowers are unable to meet repayment obligations.

Payment Time: We assess how the duration of loan repayment influences the likelihood of default. Longer repayment periods may increase the risk of a loan becoming a bad loan.

Aggregated Data: Data is aggregated to calculate key metrics, such as the number of customers and total loan amounts, which are essential for understanding trends and patterns.

Data Visualization: Visualizations, including bar charts and line graphs, are used to present findings clearly. These visual tools help in identifying patterns and making informed decisions.

Risk Mitigation: The project explores strategies to reduce default risks, such as improving credit scoring models and adjusting loan terms based on analysis.

Working Capital: Efficient management of working capital is highlighted as it relates to optimizing cash flow and reducing financial risk in lending operations.

Supply Chain Finance (SCF): We evaluate SCF solutions to understand their impact on cash flow and working capital, providing insights into optimizing financial operations.

Export / ECA Finance and Trade Loans: The project includes analysis of financing options for exporters and trade-related activities, assessing their influence on credit risk.)

### Exploratory Data Analysis

**Applicants by Loan Status** :  
<img src="./image/loan_status.png" alt="dashboard" width = "600"/>

- The majority of loan status distribution is current 47.95%, and fully paid 39.54%, it means that the borrower are meeting their payment obligation.
- There are significant number of charged off 9.08%. It means that the borrower has become delinquent on payments, and potential financial loss from the lender.
- Good loan status is either current and fully paid
- Bad loan status except for these 2 things

**Applicants by Borrower’s Status Rate** :  
<img src="./image/status.png" alt="dashboard" width = "300"/>

- Good loan status got high percentage with 87.49%. It means that the bank's loan performing is good.
- Bad loan status got low percentage with 12.51%. It means the bank need to analyzing the characteristic of the borrower, so they could
  identify early warnings sign, and implement the mitigation from failure of pay loans from customers

**Applicants by Loan Purpose** :  
<img src="./image/purpose.png" alt="dashboard" width = "600"/>

- Debt consolidation got the highest percentage for load purpose with 58.67%.
- Debt consolidation is preferred because the customer can taking out a single loan or credit card to pay off multiple debts
- The benefits of debt consolidation include a potentially lower interest rate and lower monthly payments.

**Applicants by Grade** :  
<img src="./image/grade.png" alt="dashboard" width = "600"/>

- Middle grade B and C got the highest percentage with 29.28% and 26.8%. It means that quality score to a loan based on a borrower's credit history, quality of the collateral, and the likelihood of repayment of the principal and interest are considered moderate
- Grade E,F,G got the lowest percentage. Grade E,F,G are high risk grade, because the likelihood that the borrower will repay the loan is low. So the loan company need to tighten the criteria for loan borrowers

**Applicants by Loan Term** :  
<img src="./image/term.png" alt="dashboard" width = "300"/>

- 36 month of loan term got the highest percentage with 72.47%. It means that short term loan are preferred by borrowers rather than long term.
- Compared to long term loans, the amount of interest paid is significantly less.
- These loans are considered less risky compared to long term loans because of a shorter maturity date.
- Short term loans are the lifesavers of smaller businesses or individuals who suffer from less than stellar credit scores

**Applicants by Home Ownership** :  
<img src="./image/home_ownership.png" alt="dashboard" width = "600"/>

- Mortgage got the highest percentage with 50.44%. The reason that mortgage customer is so many because a mortgage allows the customer to purchase a home without paying the full purchase price in cash.
- The second highest is rent with 40.35%. The reason that customer choose rent because no maintenance costs or repair bills, access to amenities like pool or fitness centre, no real estate taxes, and more flexibility as to where to live.
- The borrower that own their houses is only 8.9%.

### Feature Engineering with Weight of Evidence (WOE) & Information Value (IV)

<img src="./image/woe.jpg" alt="dashboard" width = "600"/>

- Weight of evidence (WOE) generally described as a measure of the separation of good and bad customers.
- Information value (IV) is one of the most useful technique to select important variables in a predictive model. It helps to rank variables on the basis of their importance.

### Modelling

**Best Parameter**  
<img src="./image/param.jpg" alt="dashboard" width = "300"/>

- Best parameter we've got is L2 (Ridge) regularization with 'C' is 0.027 which is near to 0, and leads to stronger regularization and a simpler model.

**ROC/AUC**  
<img src="./image/roc.jpg" alt="dashboard" width = "500"/>

- AUC score = 0.93, which is near to 1, indicates good performance

**Classification Report**
<img src="./image/class_report.jpg" alt="dashboard" width = "500"/>

- Precision tells us the accuracy of positive predictions. Out of all the loan status that the model predicted would get good loan, only 85% actually did.
- Recall tells us the fraction of correctly identified positive predictions. Out of all the loan status that actually did get good loan, the model only predicted this outcome correctly for 65% of those loan status
- F1 Score = 0.73. So the model does a good job of predicting whether the loan status is considered good or bad

**Confusion Matrix**  
<img src="./image/confusion_matrix.jpg" alt="dashboard" width = "500"/>

- Correct classifications are the diagonal elements of the matrix 120,440 for the positive class and 10,841 for the negative class
- Accuracy rate, which is the percentage of times a classifier is correct = 94.09%

**Kolmogorov-Smirnov**
<img src="./image/ks.jpg" alt="dashboard" width = "500"/>

- KS Statistic = 0.736. Considered it as 'medium' dataset, which mean even though it doesn't have perfect separation, but there is enough overlap to confuse the classifier, and has wide gap between the class CDF (positive & negative instances).

### Score Card

**FICO Score**  
<img src="./image/fico_score.jpg" alt="dashboard" width = "500"/>

- FICO score is a credit score created by the Fair Isaac Corporation (FICO)
- Lenders use borrowers’ FICO scores along with other details on borrowers’ credit reports to assess credit risk and determine whether to extend credit.

**Top 5 Highest & Lowest Score Features**  
<img src="./image/top_high.jpg" alt="dashboard" width = "500"/>

<img src="./image/top_low.jpg" alt="dashboard" width = "500"/>
  
Features that make contribution to increase or decrease credit score are:
- initial list status
- last payment amount
- total payment
- loan amount
- payment time

**Bad Loan Rate on Loan Amount Based On Borrower's Score Status**  
<img src="./image/bad_loan_amount.jpg" alt="dashboard" width = "600"/>

- Customers who have a bad credit score with a loan amount ranging from 465-10,850 have the potential to become a bad loan in the future

**Bad Loan Rate on Payment Time Based On Borrower's Score Status**  
<img src="./image/bad_loan_time.jpg" alt="dashboard" width = "600"/>

- The longer the customer's payment time takes to pay off the loan, the riskier customer's gonna potentially to be bad loan

### Recommendation

- Loan companies can build a robust and effective credit scoring model machine learning using variety of methods and criteria to assess the creditworthiness of potential customers.
- The goal is to minimize the risk of lending to individuals who are unlikely to repay their loans.
- One of method to evaluate a borrower incorporates both qualitative and quantitative measures is the 5 C's of credit (Character, Capacity, Capital, Collateral, and Conditions)
