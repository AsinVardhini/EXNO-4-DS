# EXNO:4-DS
# AIM:
To read the given data and perform Feature Scaling and Feature Selection process and save the
data to a file.

# ALGORITHM:
STEP 1:Read the given Data.
STEP 2:Clean the Data Set using Data Cleaning Process.
STEP 3:Apply Feature Scaling for the feature in the data set.
STEP 4:Apply Feature Selection for the feature in the data set.
STEP 5:Save the data to the file.

# FEATURE SCALING:
1. Standard Scaler: It is also called Z-score normalization. It calculates the z-score of each value and replaces the value with the calculated Z-score. The features are then rescaled with x̄ =0 and σ=1
2. MinMaxScaler: It is also referred to as Normalization. The features are scaled between 0 and 1. Here, the mean value remains same as in Standardization, that is,0.
3. Maximum absolute scaling: Maximum absolute scaling scales the data to its maximum value; that is,it divides every observation by the maximum value of the variable.The result of the preceding transformation is a distribution in which the values vary approximately within the range of -1 to 1.
4. RobustScaler: RobustScaler transforms the feature vector by subtracting the median and then dividing by the interquartile range (75% value — 25% value).

# FEATURE SELECTION:
Feature selection is to find the best set of features that allows one to build useful models. Selecting the best features helps the model to perform well.
The feature selection techniques used are:
1.Filter Method
2.Wrapper Method
3.Embedded Method

# CODING AND OUTPUT:
```
Name : Asin Vardhini R
Register Number : 212222100007
```

```
import pandas as pd
from scipy import stats
import numpy as np
df=pd.read_csv("/content/bmi.csv")

df.head()
df.dropna()
```
![image](https://github.com/user-attachments/assets/ff7841c3-ea9d-4a2d-b2d5-984a8ef9e1dd)

```
max_vals=np.max(np.abs(df[['Height']]))
max_vals
max_vals1=np.max(np.abs(df[['Weight']]))
max_vals1
print("Height =",max_vals)
print("Weight =",max_vals1)
```
![Screenshot 2024-10-08 160759](https://github.com/user-attachments/assets/6cec529f-5068-4bd6-9cbe-76b7caf25c44)


# RESULT:
       # INCLUDE YOUR RESULT HERE
