# Practical 7: Regression and ANOVA

## Aim
Simple regressions and one-way ANOVA on the Teaching Ratings data, calculated with NumPy and SciPy.

## How to run
Open practical_07.ipynb in Jupyter Notebook or Google Colab and choose Run All. Requires pandas, numpy, scipy, matplotlib, seaborn and scikit-learn.

## Output
```
Q1. eval ~ gender
Intercept (female mean): 3.9010
Male coefficient: 0.1680
R-squared: 0.022, F: 10.56, p-value: 0.00124
Decision: Reject H0, gender is significant

Q2. ANOVA: beauty ~ age group
            df      sum_sq   mean_sq          F    p
age_group    2   17.800717  8.900359  15.189048  0.0
Residual   460  269.547179  0.585972        NaN  NaN
p-value: 4.094e-07
Decision: Reject H0, beauty differs by age group

Q3. eval ~ beauty
Intercept: 3.9983
Beauty coefficient: 0.1330
R-squared: 0.036, F: 17.08, p-value: 0.000042
Decision: Reject H0, beauty is significant

Result: male instructors score about 0.168 higher, beauty differs across age groups,
and each unit of beauty adds about 0.133 to the evaluation score.
```

## Plots
All plots are shown inside the notebook.

## Result
```
Result: male instructors score about 0.168 higher, beauty differs across age groups,
and each unit of beauty adds about 0.133 to the evaluation score.
```
