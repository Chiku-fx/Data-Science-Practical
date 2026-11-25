# Practical 9: K-Nearest Neighbours

## Aim
KNN classification of Iris with scaling, error rate against K, best K and decision regions.

## How to run
Open practical_09.ipynb in Jupyter Notebook or Google Colab and choose Run All. Requires pandas, numpy, scipy, matplotlib, seaborn and scikit-learn.

## Output
```
   sepal_length  sepal_width  petal_length  petal_width species
0           5.1          3.5           1.4          0.2  setosa
1           4.9          3.0           1.4          0.2  setosa
2           4.7          3.2           1.3          0.2  setosa
3           4.6          3.1           1.5          0.2  setosa
4           5.0          3.6           1.4          0.2  setosa
<class 'pandas.DataFrame'>
RangeIndex: 150 entries, 0 to 149
Data columns (total 5 columns):
 #   Column        Non-Null Count  Dtype  
---  ------        --------------  -----  
 0   sepal_length  150 non-null    float64
 1   sepal_width   150 non-null    float64
 2   petal_length  150 non-null    float64
 3   petal_width   150 non-null    float64
 4   species       150 non-null    str    
dtypes: float64(4), str(1)
memory usage: 6.0 KB
       sepal_length  sepal_width  petal_length  petal_width
count      150.0000     150.0000      150.0000     150.0000
mean         5.8433       3.0573        3.7580       1.1993
std          0.8281       0.4359        1.7653       0.7622
min          4.3000       2.0000        1.0000       0.1000
25%          5.1000       2.8000        1.6000       0.3000
50%          5.8000       3.0000        4.3500       1.3000
75%          6.4000       3.3000        5.1000       1.8000
max          7.9000       4.4000        6.9000       2.5000
            sepal_length  sepal_width  petal_length  petal_width
species                                                         
setosa             5.006        3.428         1.462        0.246
versicolor         5.936        2.770         4.260        1.326
virginica          6.588        2.974         5.552        2.026

Confusion matrix (K=5):
[[10  0  0]
 [ 0 10  0]
 [ 0  2  8]]
Accuracy: 0.9333
              precision    recall  f1-score   support

      setosa       1.00      1.00      1.00        10
  versicolor       0.83      1.00      0.91        10
   virginica       1.00      0.80      0.89        10

    accuracy                           0.93        30
   macro avg       0.94      0.93      0.93        30
weighted avg       0.94      0.93      0.93        30

K =  1  error = 0.0333
K =  2  error = 0.0667
K =  3  error = 0.0667
K =  4  error = 0.0667
K =  5  error = 0.0667
K =  6  error = 0.0667
K =  7  error = 0.0333
K =  8  error = 0.0667
K =  9  error = 0.0333
K = 10  error = 0.0333
K = 11  error = 0.0333
K = 12  error = 0.0333
K = 13  error = 0.0333
K = 14  error = 0.0333
K = 15  error = 0.0333
K = 16  error = 0.0333
K = 17  error = 0.0333
K = 18  error = 0.0333
K = 19  error = 0.0333
K = 20  error = 0.0333
K = 21  error = 0.0333
K = 22  error = 0.0667
K = 23  error = 0.0667
K = 24  error = 0.1000
K = 25  error = 0.1000
K = 26  error = 0.1333
K = 27  error = 0.1333
K = 28  error = 0.1333
K = 29  error = 0.1333
K = 30  error = 0.1333

Lowest error: 0.0333
Odd K values with that error: [1, 7, 9, 11, 13, 15, 17, 19, 21]
Chosen K: 13
Accuracy with K=13: 0.9667

Result: K=5 gives 93.33% accuracy; the chosen K gives the final accuracy printed above.
```

## Plots
All plots are shown inside the notebook.

## Result
```
Result: K=5 gives 93.33% accuracy; the chosen K gives the final accuracy printed above.
```
