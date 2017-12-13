Statistical Analysis report
1.correlation analysis
There are more than 30 pairs of numeric variables highly correlate. Among them funded_amnt/loan_amnt funded_amnt_inv/loan_amnt and funded_amnt_inv/funded_amnt's correlation coefficient are close to 1.

2.Chi squrare test for the loan status and employment title
Hypothesis
H 0 : In the population, variable'loan_status' and variable 'emp_title' are independent.
H 1 : In the population, variable'loan_status' and variable 'emp_title' are dependent. 

Test statistics
chi_squared_stat: 269.3493768308436
Critical value: 21.0260698175 
P value: 0.0

Conclusion:
We reject H 0 and consider variable'loan_status' and variable 'emp_title are dependent. In other words loan status dependend on what kind of employment title of the borrowers.


3.Chi square test for loan status and home ownership
Hypothesis
H 0 : In the population, variable'loan_status' and variable 'home_ownership' are independent. 
H 1 : In the population, variable'loan_status' and variable 'home_ownership' are dependent.

Test Statistics
chi_squared_stat: 1692.8473338733406 
Critical value: 11.0704976935 
P value: 0.0

Conclusion:
We reject H 0 and consider variable'loan_status' and variable 'home_ownership' are dependent. It means loan status dependend on whether borrowers are renting a home or have purchased house.

4.Kruskal-Wallis H-test for the median of employment length of different loan status
The Kruskal-Wallis H-test tests the null hypothesis that the population median of all of the groups are equal. It is a non-parametric version of ANOVA. The test works on 2 or more independent samples, which may have different sizes. Note that rejecting the null hypothesis does not indicate which of the groups differs. Post-hoc comparisons between groups are required to determine which groups are different.

Hypothersis:
H 0: The population median of employment length in good loan borrowers and bad loan borrowers are equal. 
H 1: The population median of employment length in good loan borrowers and bad loan borrowers are not equal.

Test statistics:
Kruskal Wallis H-test test: 
H-statistic: 189435635.441 
P-Value: 0.0

Conclusion:We reject H 0 and consider the population median of employment length in good loan borrowers and bad loan borrowers are equal. The median of good loan borrowers' employment length is higher than that of bad loan borrowers.

5.Two sample t-test for the mean of unemployment rate in good loan borrowers and bad loan borrowers
Hypothesis:
H 0: The population mean of unemployment rate of good loan borrowers and bad loan borrowers are equal. 
H 1: The population mean of unemployment rate of good loan borrowers and bad loan borrowers are not equal.

Test statistics:
ttest_ind: t = -9.58285 p = 9.71499e-22

Conclusions:
We reject H0 and consider the mean of unemployment rate of good loan borrowers is lower than that of the bad loan borrowers.