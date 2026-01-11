# CREDIT RATING PERFORMANCE - PYTHON

## BUSINESS PROBLEM
To assess whether a loan is potentially risky or not, banks or financial institutions must evaluate many factors such as the financial health of the borrower, the loan amount, interest rates, ... Generally, banks usually classify loans into grades for easier monitoring.

This project analyzes a consumer loan dataset to evaluate the performance of the internal credit rating system 'sub_grade'. The main objective is to assess whether the rating grades from A1 to G5 effectively discriminate credit risk by examining actual default rate across different grades.

## DATASET
Description: CREDIT_RATING.CSV includes
- 31963 rows (no duplicate, 1087 missing values in 'emp_title' column)
- 18 columns (id, address_state, emp_length, emp_title, home_ownership, loan_status, member_id, purpose, sub_grade, term, ...)

Source: https://www.kaggle.com/datasets/nezukokamaado/auto-loan-dataset/data

## WHAT I DID:
**ETL:** 
- Imported and cleaned dataset, removal of outliers.
- Converted data types and created new variables to support analysis.

**EDA:**
- Created new parameters and build tables to calculate losses and risk ratios for loan defaults. 
- Visualizations primarily consist of various chart types (column, stacked column, line, boxplot, etc.) that easily illustrate customer behavior insights.
- Provided insightful observations combined with recommendations to help reduce risk and improve the accuracy of the scale in the future.

## INSIGHTS:
- Abnormally high credit risk in the portfolio. Concentration Risk in Debt Consolidation, Untapped Potential in Home Improvement.
- Linear interest rate increases perfectly offset rising risk, showing strong pricing discipline. Volatile default rates in F-G reveal loss of scoring stability and accuracy at the high-risk tail.
- DTI is a stronger predictor of creditworthiness than income. High defaults paired with large loan sizes in lower grades create outsized loss potential.

## RECOMMENDATIONS:
- Tighten underwriting standards: Focus on excluding or limiting low-income and moderate-DTI applicants to reduce overall PD.
- Strengthen debt collection: Invest in early intervention, multi-channel recovery, and specialized teams to lower LGD below 50%.
- Ensure clear rate differentiation across all grades, especially adding term-based adjustments in high-risk tiers.
- Restrict volume and loan sizes in F-G grades to control outsized loss potential. Add new criteria to improve the scale: Payment history, Transaction history, ... or switch to a point-based format to enhance quality.
