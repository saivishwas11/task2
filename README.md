# task 2

## Data Loading and Description

The dataset is loaded from the file "Titanic-Dataset.csv". The first few rows and the columns and their data types are displayed.  The dataset contains information about passengers, including:

* **PassengerId:** Unique identifier for each passenger.
* **Survived:** Indicates whether the passenger survived (0 = No, 1 = Yes).
* **Pclass:** Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd).
* **Name:** Passenger name.
* **Sex:** Passenger sex.
* **Age:** Passenger age.
* **SibSp:** Number of siblings/spouses aboard.
* **Parch:** Number of parents/children aboard.
* **Ticket:** Ticket number.
* **Fare:** Fare paid for the ticket.
* **Cabin:** Cabin number.
* **Embarked:** Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

## Data Cleaning and Preprocessing

* Missing values in the 'Age' column are imputed with the median age.
* Missing values in the 'Embarked' column are filled with the most frequent value ('S').
* The columns 'PassengerId', 'Name', 'Ticket', and 'Cabin' are dropped as they are not relevant for the analysis.

## Exploratory Data Analysis

1.  **Correlation Matrix:**
    * 'Fare' and 'Pclass' are negatively correlated (-0.55).
    * 'Age' and 'Pclass' are also negatively correlated (-0.37).
    * 'SibSp' and 'Parch' are positively correlated (0.41).

2.  **Survival Analysis:**
    * Survival rate is higher for females compared to males.
    * Survival rate is higher for passengers in first class compared to other classes.

3.  **Age Distribution:**
    * The age distribution is roughly normal, with a peak around 20-30 years.

4.  **Fare Distribution:**
     * Fare distribution is right-skewed, with most passengers paying lower fares.

5.  **Numeric Features:**
    * Boxplots show outliers in 'Fare' and 'Age'.
    * 'SibSp' and 'Parch' have many zero values.

## Visualizations

* Histograms of 'Age' and 'Fare' to visualize their distributions.
* Count plots of categorical variables ('Survived', 'Pclass', 'Sex', 'Embarked') to show their frequencies.
* Boxplots to visualize the distribution of 'Age' and 'Fare'.
* Heatmap to visualize the correlation matrix of numerical features.
* Stacked bar charts to visualize survival rate by sex and passenger class.
* Violin plots to visualize the distribution of age by passenger class and survival status.

## Summary

The analysis provides insights into the characteristics of the passengers and factors influencing their survival. Key findings include:

* Females and first-class passengers had higher survival rates.
* Age distribution is roughly normal, with most passengers aged 20-30.
* Fare distribution is right-skewed, indicating that most passengers paid lower fares.
* There is a negative correlation between Fare and Pclass, and Age and Pclass.
