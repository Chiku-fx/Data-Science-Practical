# Practical 5: Probability and z-test

## Aim
Normal probabilities for evaluation scores and a two-tailed z-test.

## How to run
Open practical_05.ipynb in Jupyter Notebook or Google Colab and choose Run All. Requires pandas, numpy, scipy, matplotlib, seaborn and scikit-learn.

## Output
```
Mean evaluation: 3.9983
Standard deviation: 0.5549

P(score > 4.5)
z = 0.9042
Normal model: 0.1829 (18.29%)
From data:    0.1706 (17.06%)

P(3.5 < score < 4.2)
z values = -0.8980, 0.3636
Normal model: 0.4573 (45.73%)
From data:    0.3542 (35.42%)

Two-tailed z-test (H0: mean = 12, alpha = 0.05)
Standard error: 0.9167
z statistic: -1.4182
p-value: 0.1561
Critical value: +/- 1.9600
Decision: Fail to reject H0

Result: P(score > 4.5) is about 18.29%, P(3.5 < score < 4.2) is about 45.73%,
and the z-test does not reject H0, so no significant difference in means is found.
```

## Plots
All plots are shown inside the notebook.

## Result
```
Result: P(score > 4.5) is about 18.29%, P(3.5 < score < 4.2) is about 45.73%,
and the z-test does not reject H0, so no significant difference in means is found.
```
