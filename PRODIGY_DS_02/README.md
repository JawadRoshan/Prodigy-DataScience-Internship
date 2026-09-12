# Titanic Dataset — Data Cleaning and Exploratory Data Analysis

## Task Objective

The objective of this task was to perform data cleaning and exploratory data analysis (EDA) on the Titanic dataset and explore relationships between different passenger attributes and their survival.

## Dataset

The dataset contains information about **891 Titanic passengers** and includes variables such as:

* Passenger class
* Gender
* Age
* Number of siblings/spouses aboard
* Number of parents/children aboard
* Fare
* Port of embarkation
* Survival status

## Data Cleaning

The dataset was inspected for missing values, duplicate records, and data types.

Missing values were found in:

* **Age:** 177 missing values
* **Cabin:** 687 missing values
* **Embarked:** 2 missing values

The following cleaning steps were performed:

* Missing `Age` values were replaced using the median age.
* Missing `Embarked` values were replaced using the most frequent value.
* The `Cabin` column was removed because a large majority of its values were missing.
* Duplicate records were checked and no duplicates were found.

After cleaning, the dataset contained **no missing values**.

---

## Exploratory Data Analysis

### 1. Overall Survival

Out of 891 passengers:

* **342 passengers survived**
* **549 passengers did not survive**

This means approximately:

* **38.38% survived**
* **61.62% did not survive**

Therefore, the majority of passengers in the dataset did not survive the Titanic disaster.

### 2. Gender and Survival

Survival rates showed a very strong relationship with gender.

* **Female survival rate:** approximately **74.20%**
* **Male survival rate:** approximately **18.89%**

Female passengers had a significantly higher survival rate than male passengers.

This suggests that gender was one of the strongest factors associated with survival in this dataset.

### 3. Passenger Class and Survival

Survival rates by passenger class were:

| Passenger Class | Survival Rate |
| --------------- | ------------: |
| 1st Class       |        62.96% |
| 2nd Class       |        47.28% |
| 3rd Class       |        24.24% |

Passengers in higher classes generally had much higher survival rates than passengers in third class.

This indicates a strong relationship between passenger class and survival.

### 4. Age and Survival

The average age of passengers was:

* **Passengers who did not survive:** approximately 30.03 years
* **Passengers who survived:** approximately 28.29 years

The difference was relatively small, around 1.74 years.

Therefore, age alone showed a much weaker relationship with survival compared with gender and passenger class.

### 5. Fare and Survival

The average fare was:

* **Non-survivors:** approximately 22.12
* **Survivors:** approximately 48.40

Survivors paid more than twice the average fare paid by non-survivors.

This is likely connected to passenger class, as first-class passengers generally paid higher fares and also had higher survival rates.

### 6. Family Relationships and Survival

The number of siblings/spouses (`SibSp`) and parents/children (`Parch`) was also explored.

Passengers travelling with a small number of family members sometimes showed higher survival rates than passengers travelling alone or in very large family groups.

However, some categories had very few passengers, so these results should be interpreted carefully.

### 7. Gender and Passenger Class Combined

The strongest pattern appeared when gender and passenger class were considered together.

Survival rates were:

| Passenger Class | Female |   Male |
| --------------- | -----: | -----: |
| 1st Class       | 96.81% | 36.89% |
| 2nd Class       | 92.11% | 15.74% |
| 3rd Class       | 50.00% | 13.54% |

First-class females had the highest survival rate, while third-class males had the lowest.

This demonstrates that survival was influenced by multiple factors rather than a single variable.

---

## Correlation Analysis

A correlation matrix was used to understand relationships between numerical variables.

The strongest correlations with `Survived` were:

* **Pclass:** -0.338
* **Fare:** +0.257
* **Parch:** +0.082
* **Age:** -0.065
* **SibSp:** -0.035

The negative correlation between `Pclass` and `Survived` occurs because the classes are represented numerically as:

* 1 = First Class
* 2 = Second Class
* 3 = Third Class

Therefore, a higher numerical class value represents a lower passenger class and is associated with lower survival.

Correlation shows association between variables and **does not prove causation**.

---

# Key Findings

The main patterns identified during the analysis were:

1. **Overall survival was relatively low**, with only 38.38% of passengers surviving.

2. **Gender was one of the strongest predictors of survival.** Female passengers had a survival rate of approximately 74.20%, compared with only 18.89% for male passengers.

3. **Passenger class had a strong relationship with survival.** First-class passengers had the highest survival rate at 62.96%, while third-class passengers had the lowest at 24.24%.

4. **Fare was positively associated with survival.** Survivors paid an average fare of approximately 48.40 compared with 22.12 for non-survivors.

5. **Age showed only a weak relationship with survival** in this dataset.

6. **Family size showed mixed patterns.** Small family groups sometimes had better survival rates, while very large groups generally showed lower rates. However, categories with very few passengers should be interpreted cautiously.

7. **Gender and passenger class together revealed an even stronger pattern.** First-class females had a survival rate of approximately 96.81%, while third-class males had a survival rate of approximately 13.54%.

---

# Conclusion

The exploratory data analysis of the Titanic dataset revealed that **survival was strongly associated with gender and passenger class**. Female passengers and passengers travelling in higher classes had substantially higher survival rates than male and third-class passengers.

Fare also showed a positive relationship with survival, which is likely connected to passenger class. In contrast, age showed only a relatively weak relationship with survival in this dataset.

The analysis demonstrates how data cleaning, visualization, grouping, and correlation analysis can be used to identify meaningful patterns within a dataset. It also highlights the importance of considering multiple variables together rather than relying on a single factor.

Overall, the Titanic dataset provides a useful example of how **exploratory data analysis can uncover relationships, patterns, and trends before applying more advanced statistical or machine-learning techniques.**

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook / Google Colab

## Project Status

**Completed — Prodigy InfoTech Data Science Internship, Task 2**
