# AIPredictionModel-TestScore
Can a computer predict a test score using study and sleep time? This project uses a simple AI model to predict a student’s test score based on hours studied and hours slept.
I am trying to see if a computer can predict a test score using study time and sleep.
The project trains a simple AI model using sample data and makes test score predictions.
Python, Pandas, Scikit-learn, Google Sheets, GitHub
The model successfully predicts realistic test scores.
I learned how data is used to train an AI model.
[data.csv](https://github.com/user-attachments/files/25191218/data.csv)
1 | 5 | 58

2 | 5 | 62

3 | 6 | 70

4 | 6 | 74

5 | 7 | 80

6 | 7 | 84

7 | 8 | 88

8 | 8 | 91

9 | 9 | 95

10 | 9 | 97 [model.py](https://github.com/user-attachments/files/25191220/model.py) 
import pandas as pd
from sklearn.linear_model import LinearRegression

"data = pd.read_csv(""data.csv"")"

"X = data[[""Hours_Studied"", ""Hours_Slept""]]"
"y = data[""Test_Score""]"

model = LinearRegression()
"model.fit(X, y)"

"prediction = model.predict([[6, 8]])"

"print(""The AI predicted a test score of "" + str(prediction[0]) +"
""" for a student who studied 6 hours and slept 8 hours."")"
The AI predicted a test score of _____ for a student
who studied 6 hours and slept 8 hours.
