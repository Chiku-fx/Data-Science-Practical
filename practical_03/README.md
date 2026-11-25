# Practical 3: Exploratory data analysis

## Aim
Tenure percentages, cross-tabulation, age summary, histogram, bar charts and median score on the Teaching Ratings data. The original evals.csv file was not available, so the equivalent Teaching Ratings data is used.

## How to run
Open practical_03.ipynb in Jupyter Notebook or Google Colab and choose Run All. Requires pandas, numpy, scipy, matplotlib, seaborn and scikit-learn.

## Output
```
<class 'pandas.DataFrame'>
RangeIndex: 463 entries, 0 to 462
Data columns (total 13 columns):
 #   Column       Non-Null Count  Dtype  
---  ------       --------------  -----  
 0   rownames     463 non-null    int64  
 1   minority     463 non-null    str    
 2   age          463 non-null    int64  
 3   gender       463 non-null    str    
 4   credits      463 non-null    str    
 5   beauty       463 non-null    float64
 6   eval         463 non-null    float64
 7   division     463 non-null    str    
 8   native       463 non-null    str    
 9   tenure       463 non-null    str    
 10  students     463 non-null    int64  
 11  allstudents  463 non-null    int64  
 12  prof         463 non-null    int64  
dtypes: float64(2), int64(5), str(6)
memory usage: 47.2 KB
       rownames       age    beauty      eval  students  allstudents      prof
count  463.0000  463.0000  463.0000  463.0000  463.0000     463.0000  463.0000
mean   232.0000   48.3650    0.0000    3.9983   36.6242      55.1771   45.4341
std    133.8008    9.8027    0.7886    0.5549   45.0185      75.0728   27.5089
min      1.0000   29.0000   -1.4505    2.1000    5.0000       8.0000    1.0000
25%    116.5000   42.0000   -0.6563    3.6000   15.0000      19.0000   20.0000
50%    232.0000   48.0000   -0.0680    4.0000   23.0000      29.0000   44.0000
75%    347.5000   57.0000    0.5456    4.4000   40.0000      60.0000   70.5000
max    463.0000   73.0000    1.9700    5.0000  380.0000     581.0000   94.0000

Minority instructors with tenure: 84.38%
All other instructors with tenure: 76.94%

Minority vs tenure:
tenure    no  yes
minority         
no        92  307
yes       10   54

Age by tenure status:
           mean      std
tenure                  
no      50.1863   6.9464
yes     47.8504  10.4201

Gender counts:
gender
male      268
female    195
Name: count, dtype: int64

Median evaluation of tenured instructors: 4.0

Result: untenured instructors are older on average, and the tenure share of minority
instructors (84.38%) is higher than that of the rest.
```

## Plots
All plots are shown inside the notebook.

## Result
```
Result: untenured instructors are older on average, and the tenure share of minority
instructors (84.38%) is higher than that of the rest.
```
