# SGD-Classifier
## AIM:
To write a program to predict the type of species of the Iris flower using the SGD Classifier.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
```
1. Start
2.Read two numbers (A, B)
3.Add A and B → Result
4.Display Result
5.Stop
```

## Program:
```
/*
Program to implement the prediction of iris species using SGD Classifier.
Developed by: hema priya
RegisterNumber:212225240051
/*



from sklearn import datasets
from sklearn.linear_model import SGDClassifier
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score

iris = datasets.load_iris()
X = iris.data
Y = iris.target

X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=0.2, random_state=0)

model = SGDClassifier(max_iter=1000, learning_rate='optimal')
model.fit(X_train, Y_train)

Y_pred = model.predict(X_test)

print("Accuracy:", accuracy_score(Y_test, Y_pred))

sample = [X[0]]
prediction = model.predict(sample)

print("Predicted Species:", iris.target_names[prediction][0])
*/
```

## Output:
```
<img width="696" height="59" alt="Screenshot 2026-04-30 143900" src="https://github.com/user-attachments/assets/07b3b11b-958e-46c5-abd6-536260d6ae77" />


```

## Result:
Thus, the program to implement the prediction of the Iris species using SGD Classifier is written and verified using Python programming.
