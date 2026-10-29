 Dataset Exploration: Titanic

 Overview
- File: data/raw_dataset.csv
- Rows: 891 passengers
- Columns: 12
- Goal: Understand the passengers and what affected survival.

 Column Schema

| Column | Data Type | Description |
|---|---|---|
| PassengerId | Numerical (integer) | Unique ID for each passenger |
| Survived | Categorical (binary) | 0 = did not survive, 1 = survived |
| Pclass | Categorical (ordinal) | Ticket class: 1 = first, 2 = second, 3 = third |
| Name | Text | Passenger's full name |
| Sex | Categorical | male or female |
| Age | Numerical (float) | Age in years |
| SibSp | Numerical (integer) | Number of siblings or spouses aboard |
| Parch | Numerical (integer) | Number of parents or children aboard |
| Ticket | Text | Ticket number |
| Fare | Numerical (float) | Price paid for the ticket |
| Cabin | Text | Cabin number |
| Embarked | Categorical | Port of boarding: C = Cherbourg, Q = Queenstown, S = Southampton |

  Missing Values

| Column | Missing Count |
|---|---|
| Age | 177 |
| Cabin | 687 |
| Embarked | 2 |

All other columns have no missing values.

 Initial Observations
- Cabin is missing for most passengers, so it is hard to use without heavy cleaning.
- Age has some gaps that could be filled with the median age.
- Survived is the likely target column for prediction.
- Sex and Pclass look important for studying survival patterns.
