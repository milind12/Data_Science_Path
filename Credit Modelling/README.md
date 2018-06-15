
# Credit Modelling
In this project we build machine learning model that reliably predict if a loan will be paid off or not.

## Dataset
You can get dataset from here https://www.lendingclub.com/info/download-data.action. To learn more about what a column represents in the datasets. Here's a link to the data dictionary file hosted on Google Drive. https://docs.google.com/spreadsheets/d/191B2yJ4H1ZPXq0_ByhUgWMFZOYem5jFz0Y3by_7YBY4/edit#gid=2081333097

## Feature Selection
From below observations, we can conclude that the following features need to be removed:
1. id: <b>randomly</b> generated field by Lending Club for unique identification purposes only
2. member_id: also a <b>randomly</b> generated field by Lending Club for unique identification purposes only
3. funded_amnt: <b>leaks data from the future </b>(after the loan is already started to be funded)
4. funded_amnt_inv: <b>also leaks data from the future</b> (after the loan is already started to be funded)
5. grade: contains <b>redundant information as the interest rate column </b>(int_rate)
6. sub_grade: also contains <b>redundant information as the interest rate column </b>(int_rate)
7. emp_title:<b> requires other data and a lot of processing to potentially be useful</b>
8. issue_d: <b> leaks data from the future</b> (after the loan is already completed funded)
9. zip_code: <b> redundant with the addr_state column </b> since only the first 3 digits of the 5 digit zip code are visible (which only can be used to identify the state the borrower lives in)
10. out_prncp: <b> leaks data from the future</b>, (after the loan already started to be paid off)
11. out_prncp_inv: <b> also leaks data from the future</b>, (after the loan already started to be paid off)
12. total_pymnt: also <b> leaks data from the future, (after the loan already started to be paid off)</b>
13. total_pymnt_inv: <b> also leaks data from the future, (after the loan already started to be paid off)</b>
14. total_rec_prncp:<b> also leaks data from the future, (after the loan already started to be paid off) </b>
15. total_rec_int: <b>leaks data from the future, (after the loan already started to be paid off)</b>,
16. total_rec_late_fee: also <b>leaks data from the future, (after the loan already started to be paid off)</b>,
17. recoveries: also <b>leaks data from the future, (after the loan already started to be paid off)</b>,
18. collection_recovery_fee: <b>also leaks data from the future, (after the loan already started to be paid off)</b>,
19. last_pymnt_d:</b> also leaks data from the future, (after the loan already started to be paid off)</b>,
20. last_pymnt_amnt: <b> also leaks data from the future, (after the loan already started to be paid off)</b>.

<b> All the columns containing only one unique value were removed.</b>

## Feature Transformation
Categorical columns with a few categorical values are encoded as dummy variable.

## Error metric
we should optimize for:
1. high recall (true positive rate)
2. low fall-out (false positive rate)

## Prediction
We can use the RandomForestClassifer class from scikit-learn for prediction.


