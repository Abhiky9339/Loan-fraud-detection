# Loan Fraud Detection

Project domain:  Banking / Loan

### Problem Statement:

##### Bussiness Objective:

ABC is a Non-Banking Financial Company (NBFC) that facilitates peer-to-peer loans, connecting individuals who need money (borrowers) with those who have money (investors). As an investor, you would want to invest in borrowers who have demonstrated a high likelihood of repayment, enabling you to confidently extend additional loans to them alongside their existing ones.

##### critical concerns: 

Ensure NPAs(Non Performing Assets) remain low – meaning ABC aims to be highly diligent in approving loans to borrowers.


##### Goals:

The goal is to develop a Classification model that predicts whether a borrower can be granted another loan based on their likelihood of repaying it. 

The primary focus is on reducing Non-Performing Assets (NPAs) while creating the model and

Expanding the borrower base.

##### Stakeholders: 

ABC company, Investors, Regulatory authorities.


### Key Performance Indicators:

1.Loan Approval Rate: Percentage of loan applications approved based on the credit policy criteria.

2.Credit Score Distribution: Distribution and analysis of FICO credit scores (fico) among borrowers and its correlation with loan performance.

3.Default Rate: Percentage of loans where the borrower did not fully pay back the loan (not.fully.paid).

4.Revolving Credit Analysis: Analysis of revolving balance (revol.bal) and utilization rate (revol.util) to understand borrower's credit utilization behavior.

5.Interest Rate Analysis: Average interest rate (int.rate) charged on loans and its impact on borrower behavior and       profitability.

6.Installment Analysis: Average and distribution of monthly installments (installment) paid by borrowers.

7.Income Analysis: Analysis of logarithm of annual income (log.annual.inc) and its impact on loan repayment rates.

8.Income vs. Debt Ratio: Analysis of debt-to-income ratio (dti) to assess borrower's financial health and risk.

9.Purpose of Loan: Distribution and analysis of loan purposes (purpose) to identify high-risk loan categories.

10.Delinquency Analysis: Frequency of delinquencies (delinq.2yrs) and its impact on loan default rates.

11.Public Records: Analysis of public records (pub.rec) and its correlation with loan repayment behavior.


### Data Description:

#### credit.policy:
Indicates whether the loan applicant meets the lending criteria set by the lender. This is often a binary variable where 1 means the applicant meets the credit policy, and 0 means they do not.

#### purpose:
The purpose of the loan, such as debt consolidation, home improvement, major purchase, etc. This is a categorical variable that describes why the applicant is requesting the loan.

#### int.rate:
The interest rate charged on the loan, expressed as a decimal. For example, an interest rate of 15% would be represented as 0.15.

#### installment:
The monthly payment that the borrower needs to make to repay the loan. It includes both principal and interest.

#### log.annual.inc:
The natural logarithm of the annual income of the borrower. Using the logarithm helps in normalizing the income data and managing large variations.

#### dti (Debt-to-Income ratio):
A measure of the borrower’s monthly debt payments divided by their monthly gross income. It helps in assessing the borrower’s ability to manage monthly payments and repay debts.

#### fico:
The borrower’s FICO credit score, which ranges typically from 300 to 850. It is a measure of the borrower’s creditworthiness.

#### days.with.cr.line:
The number of days the borrower has had a credit line. This is a measure of the length of the borrower’s credit history.

#### revol.bal (Revolving balance):
The amount of money owed by the borrower on revolving credit accounts, such as credit cards.

#### revol.util (Revolving line utilization rate):
The ratio of the borrower’s revolving balance to their credit limit, expressed as a percentage. It measures how much of the available credit is being used by the borrower.

#### inq.last.6mths:
The number of inquiries made into the borrower’s credit report by lenders in the last 6 months. Multiple inquiries can indicate a higher risk as it might suggest the borrower is seeking multiple lines of credit.

#### delinq.2yrs:
The number of times the borrower has been 30 or more days past due on a payment in the past 2 years.

#### pub.rec (Public records):
The number of derogatory public records (e.g., bankruptcies, tax liens, or judgments) associated with the borrower’s credit history.

#### not.fully.paid:
Indicates whether the borrower has not fully paid back the loan. This is often a binary variable where 1 means the loan was not fully paid, and 0 means it was fully paid.

#### loan_approved: 
Indicates whether the loan has been approved or not based on the above criteries. This is binaru variable where 1 being loan has been approved and 0 being loan is not approved

### Observations:
The following observations were made during the project period:

1. The historical loan data from ABC NBFC is a valuable resource for predicting loan fraud detection.
2. Various classification algorithms can be employed to predict loan approval status.
3. Model performance can be enhanced through feature engineering and hyperparameter tuning.

### Conclusion:

After analyzing the historical loan data from ABC NBFC, we successfully developed a model to predict loan fraud detection. By transforming the categorical values to 'Approved' and 'Not Approved' based on the 'loan approved' column and renaming this column to 'Loan Approval Status', we enhanced the readability and identification of loan statuses in the original dataset. 

Among the various classification algorithms tested, the Random Forest model emerged as the best fit for predicting loan fraud. This model demonstrated superior accuracy and reliability, effectively distinguishing between legitimate and fraudulent loan applications. The use of feature engineering and hyperparameter tuning further improved the model's performance, making it a robust tool for identifying loan fraud and ensuring more secure loan approval processes.







