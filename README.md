# Data Cleaning Portfolio

Welcome to my portfolio showcasing data cleaning skills for freelancing. Starting with beginner projects using Excel and public datasets.

## Titanic Dataset Cleaning Project

### Overview
This project uses the Titanic passenger dataset from Kaggle, which includes 891 rows of data on passengers from the 1912 disaster.
Key columns: PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked.
Main issues addressed: Missing values (e.g., 177 in Age, 687 in Cabin), potential duplicates, inconsistent formatting, and outliers in Age/Fare.
Goal: Produce a clean dataset ready for analysis, demonstrating skills in data imputation, standardization, and validation using Excel.

### Before/After Summary
| Issue | Before | After | Method Used |
|-------|--------|-------|-------------|
| Missing Age | 177 blanks | Filled with median (28) | Median imputation |
| Missing Cabin | 687 blanks | Column dropped | Too sparse for use |
| Missing Embarked | 2 blanks | Filled with 'S' | Mode (most common) |
| Duplicates | 0 | 0 | Checked and none found |
| Outliers in Fare | Some >$200 | Capped at upper IQR bound (~$65) | IQR method |
| Formats | Mixed case in Sex/Embarked | Standardized (lowercase Sex, uppercase Embarked) | Formulas like LOWER/UPPER |

### Steps Explained
- Handled missing Age with =MEDIAN() and IF(ISBLANK() formula.
- Dropped Cabin column via delete.
- Standardized formats using LOWER() and UPPER() functions.
- Detected outliers with QUARTILE.INC() for IQR.

### Files in This Repo
- [Titanic_Cleaning_Project.xlsx](Titanic_Cleaning_Project.xlsx): Cleaned data + documentation.
- [train.csv](train.csv): Original raw dataset.
- Images: Screenshots of before/after.

### Insights
After cleaning, average age is ~29.7, and survival rate is 38%—data now ready for further analysis.

## Future Projects
Planning to add more, like Airbnb or sales data cleaning.

Contact: [https://www.linkedin.com/in/jyotiraditya-chavan-4557a9285/]
