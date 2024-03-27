## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import pandas for data manipulation and sklearn for machine learning operations. 2.Load data from a CSV file using pandas, then preprocess it by removing unnecessary columns and handling missing values if any. 3.Divide the preprocessed data into training and testing sets. 4.Train a machine learning model, such as logistic regression (lr), on the training data. 5.Calculate accuracy, generate confusion matrix, and produce a classification report to assess model performance. 6.Utilize the trained model to make predictions on new data points, ensuring it's fitted on training data before predicting on the test set.

## Program:
```
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: MONISH R
RegisterNumber:  212223220061
*/
import pandas as pd
data = pd.read_csv("/content/Placement_Data.csv")
data.head()
data1=data.copy()
data1=data1.drop(["sl_no","salary"],axis=1)
data1.head()
data1.isnull().sum()
data1.duplicated().sum()
x=data1.iloc[:,:-1]
x
y=data1["status"]
y
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.metrics import accuracy_score
accuracy = accuracy_score(y_test,y_pred)
accuracy
from sklearn.metrics import confusion_matrix
confusion = (y_test,y_pred)
confusion
from sklearn.metrics import classification_report
classification_report1 = classification_report(y_test,y_pred)
print(classification_report1)
lr.predict([[1,80,1,90,1,1,90,1,0,85,1,85]])
```

## Output:
![314367688-32d647e7-f70f-4fba-a8e6-8b16201c475c](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/06586fbf-a118-4e0b-8192-442848a30bc3)
![314367740-2f62e9d3-7684-44e8-a969-4eddcbe808d3](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/a53e1002-be1f-4af2-87aa-fb0f1ff4aaea)
![314367779-e2633c37-45a7-4b28-83f1-77ab15765e1e](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/f647426a-7250-49a3-b822-b6c7d9e4c2a5)
![314367834-38361f24-94ec-42de-aa6e-14d67d3304ad](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/9d6d0f55-96e2-4ab0-8d2a-605118ce1dd1)
![314367896-89fee1bc-aabc-4868-b12e-7019d1f117da](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/2e76caa1-85db-43fb-b12b-a616aa740911)
![314368328-41b02477-baa5-487c-9c06-264d895097da](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/03ba112e-fec5-423a-851c-938af0148859)
![314368412-637b03a9-3ad4-4390-8dc4-7ccd82119d9f](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/1fbbdc1a-e1ab-4490-a381-c67a4cceb77a)
![314368575-42e96505-13fb-457d-9d81-d76d1486d5a9](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/3dcf9cdc-8f3e-4964-ad9b-92642afed361)
![314368600-5e57cad1-6a4d-409b-a63d-a71657d5d2f2](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/bd781353-0e8a-437c-9a21-1fe8fdf62827)
![314368653-75502ec7-8b17-40dd-a575-db8c6d0e6e97](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/1e717203-9f79-450c-ad6a-4dfb1c493ea3)
![314368690-9baf5590-6c48-4a0f-8162-111459350534](https://github.com/monishr288/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/147474049/02fa2f10-b860-4c34-a1a9-43ba81d47135)

## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
