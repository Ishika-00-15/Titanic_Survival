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

There are 891 values under each coloum with missing values in columns 'Age', 'Cabin' and 'Embarked'. We have imputed the missing values in 'Age' column using the median age and the missing values of'Embarked' column withtthe most frequent value. 
