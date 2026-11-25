# Practical 1: NumPy and Pandas basics

## Aim
Load the Students Performance data, convert it to arrays, check shape/size/dimensions, and apply matrix operations.

## How to run
Open practical_01.ipynb in Jupyter Notebook or Google Colab and choose Run All. Requires pandas, numpy, scipy, matplotlib, seaborn and scikit-learn.

## Output
```
Rows and columns: (1000, 8)
gender                           str
race/ethnicity                   str
parental level of education      str
lunch                            str
test preparation course          str
math score                     int64
reading score                  int64
writing score                  int64
dtype: object

Shape: (1000, 3)
Size: 3000
Dimensions: 2

Selected rows:
   math score  reading score
0          72             72
1          69             90
2          90             95
3          47             57

First matrix:
[[72 72]
 [69 90]]
Second matrix:
[[90 95]
 [47 57]]

Addition:
[[162 167]
 [116 147]]
Subtraction:
[[-18 -23]
 [ 22  33]]
Element-wise multiplication:
[[6480 6840]
 [3243 5130]]
Matrix product:
[[ 9864 10944]
 [10440 11685]]
Inverse of first matrix:
[[ 0.0595 -0.0476]
 [-0.0456  0.0476]]
Transpose of first matrix:
[[72 69]
 [72 90]]

Shape after one-hot encoding: (1000, 20)
   math score  reading score  ...  race/ethnicity_group B  race/ethnicity_group C
0          72             72  ...                       1                       0
1          69             90  ...                       0                       1
2          90             95  ...                       1                       0

[3 rows x 8 columns]

Result: the data was converted to arrays and all matrix operations ran successfully.
```

## Plots
All plots are shown inside the notebook.

## Result
```
Result: the data was converted to arrays and all matrix operations ran successfully.
```
