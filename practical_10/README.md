# Practical 10: Principal Component Analysis

## Aim
Statistics, boxplots, scatter plot, covariance matrix, scaling and PCA on the Wine data.

## How to run
Open practical_10.ipynb in Jupyter Notebook or Google Colab and choose Run All. Requires pandas, numpy, scipy, matplotlib, seaborn and scikit-learn.

## Output
```
Shape: (178, 14)
Classes: [np.int64(1), np.int64(2), np.int64(3)]
                              count     mean  ...      75%      max
alcohol                       178.0   13.001  ...   13.678    14.83
malic_acid                    178.0    2.336  ...    3.082     5.80
ash                           178.0    2.367  ...    2.558     3.23
alcalinity_of_ash             178.0   19.495  ...   21.500    30.00
magnesium                     178.0   99.742  ...  107.000   162.00
total_phenols                 178.0    2.295  ...    2.800     3.88
flavanoids                    178.0    2.029  ...    2.875     5.08
nonflavanoid_phenols          178.0    0.362  ...    0.438     0.66
proanthocyanins               178.0    1.591  ...    1.950     3.58
color_intensity               178.0    5.058  ...    6.200    13.00
hue                           178.0    0.957  ...    1.120     1.71
od280/od315_of_diluted_wines  178.0    2.612  ...    3.170     4.00
proline                       178.0  746.893  ...  985.000  1680.00
class                         178.0    1.938  ...    3.000     3.00

[14 rows x 8 columns]

Covariance matrix (first 5 columns):
                   alcohol  malic_acid    ash  alcalinity_of_ash  magnesium
alcohol              0.659       0.086  0.047             -0.841      3.140
malic_acid           0.086       1.248  0.050              1.076     -0.871
ash                  0.047       0.050  0.075              0.406      1.123
alcalinity_of_ash   -0.841       1.076  0.406             11.153     -3.975
magnesium            3.140      -0.871  1.123             -3.975    203.989

Scaled mean: [-0.]
Scaled std: [1.]

First rows of PCA output:
      PC1     PC2  class
0  3.3168  1.4435      1
1  2.2095 -0.3334      1
2  2.5167  1.0312      1
3  3.7571  2.7564      1
4  1.0089  0.8698      1
Explained variance ratio: [0.362  0.1921]
Total variance explained: 55.41%

Result: two components keep 55.41% of the variance and separate the three wine classes well.
```

## Plots
All plots are shown inside the notebook.

## Result
```
Result: two components keep 55.41% of the variance and separate the three wine classes well.
```
