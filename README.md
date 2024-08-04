# Titanic_Survival

The dataset contains the following columns:

    PassengerId: Unique identifier for each passenger.
    Survived: Whether the passenger survived (1) or not (0).
    Pclass: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd).
    Name: Name of the passenger.
    Sex: Gender of the passenger.
    Age: Age of the passenger.
    SibSp: Number of siblings or spouses aboard the Titanic.
    Parch: Number of parents or children aboard the Titanic.
    Ticket: Ticket number.
    Fare: Ticket fare.
    Cabin: Cabin number.
    Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

There are 891 values under each coloum with missing values in columns 'Age', 'Cabin' and 'Embarked'. We have imputed the missing values in 'Age' column using the median age and the missing values of'Embarked' column with the most frequent value. 
From the pie chart, we observe that only 38.4% and the bar chart confirms that most of the casualities are from the third class. 
Running logistic regression with 'Survived' as the dependent variable and train data to test data split to be 8:2, we find the accuracy to be 81.01%. This implies that the model correctly predicted the survival status of passengers 81.01% of the time on the test set.
Now, confusion matrix is a table used to evaluate the performance of a classification algorithm. It provides a detailed breakdown of the model's predictions, showing how many instances were correctly or incorrectly classified for each class. The matrix has four main components:
   
	90: True negatives (correctly predicted non-survivors)
	15: False positives (incorrectly predicted survivors)
	19: False negatives (incorrectly predicted non-survivors)
	55: True positives (correctly predicted survivors)

The confusion matrix shows that the model correctly identifies most of the actual survivors and non-survivors, with relatively few misclassifications.

Moreover, the classification report suggests that it has a slightly higher recall for non-survivors (86%) than for survivors (74%), indicating it is better at correctly identifying non-survivors.
Precision is also slightly higher for non-survivors (83%) than for survivors (79%), suggesting the model makes fewer false positive errors for non-survivors.
The balanced F1-scores indicate that the model maintains a good balance between precision and recall for both classes.
Overall, the model demonstrates good performance in predicting the survival status of Titanic passengers.
