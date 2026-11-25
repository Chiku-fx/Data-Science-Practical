# Practical 6: Statistical tests

## Aim
T-test, ANOVA, chi-square test and Pearson correlation.

## How to run
Open practical_06.ipynb in Jupyter Notebook or Google Colab and choose Run All. Requires pandas, numpy, scipy, matplotlib, seaborn and scikit-learn.

## Output
```
1. T-test: gender and evaluation
Male mean 4.0690 (n=268), female mean 3.9010 (n=195)
t = 3.2667, p = 0.0012
Decision: Reject H0, gender affects evaluation

2. ANOVA: beauty and age group
Q1 mean beauty 0.3426 (n=136)
Q2 mean beauty -0.1051 (n=97)
Q3 mean beauty -0.1049 (n=136)
Q4 mean beauty -0.2354 (n=94)
F = 13.7820, p = 0.00000001
Decision: Reject H0, beauty differs by age group

3. Chi-square: gender and tenure
tenure  no  yes
gender         
female  50  145
male    52  216
chi2 = 2.2068, dof = 1, p = 0.1374
Decision: Fail to reject H0, no association

4. Correlation: beauty and evaluation
r = 0.1890, p = 0.00004247
Decision: Reject H0, significant positive correlation

Result: gender, age group and beauty each show a significant effect;
gender and tenure are not significantly associated.
```

## Plots
All plots are shown inside the notebook.

## Result
```
Result: gender, age group and beauty each show a significant effect;
gender and tenure are not significantly associated.
```
