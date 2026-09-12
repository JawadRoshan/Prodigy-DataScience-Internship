# Task 2 — Exploratory Data Analysis on Titanic Dataset

## Key Findings

The Titanic dataset was analyzed to understand the factors associated with passenger survival.

### 1. Overall Survival

* Total passengers analyzed: **891**
* Passengers who survived: **342 (38.38%)**
* Passengers who did not survive: **549 (61.62%)**
* Therefore, the majority of passengers in the dataset did not survive.

### 2. Gender and Survival

Gender showed one of the strongest relationships with survival.

* **Female survival rate:** 74.20%
* **Male survival rate:** 18.89%

Female passengers had a significantly higher survival rate than male passengers.

### 3. Passenger Class and Survival

Passenger class also showed a clear relationship with survival.

* **1st Class:** 62.96%
* **2nd Class:** 47.28%
* **3rd Class:** 24.24%

Passengers in higher classes generally had higher survival rates, while 3rd-class passengers had the lowest survival rate.

### 4. Gender and Passenger Class Combined

The combination of gender and passenger class revealed an even stronger pattern:

| Passenger Class | Female Survival | Male Survival |
| --------------- | --------------: | ------------: |
| 1st Class       |          96.81% |        36.89% |
| 2nd Class       |          92.11% |        15.74% |
| 3rd Class       |          50.00% |        13.54% |

1st-class females had the highest survival rate, while 3rd-class males had the lowest.

This suggests that gender and passenger class together were strongly associated with survival outcomes.

### 5. Age and Survival

The average age was:

* **Non-survivors:** 30.03 years
* **Survivors:** 28.29 years

The difference was relatively small, suggesting that **age alone did not show a strong relationship with survival** in this analysis.

### 6. Fare and Survival

Average fare:

* **Non-survivors:** 22.12
* **Survivors:** 48.40

Survivors paid considerably higher fares on average. This is likely related to passenger class, as higher-class passengers generally paid higher fares and also had higher survival rates.

### 7. Family Relationships and Survival

The number of siblings/spouses and parents/children aboard showed some variation in survival rates.

Passengers traveling with a small number of family members sometimes had higher survival rates than passengers traveling alone or in very large family groups.

However, categories with very few passengers can produce misleading percentages, so these results should be interpreted cautiously.

### 8. Correlation Analysis

The correlation analysis showed the following relationships with survival:

* **Pclass:** -0.338
* **Fare:** +0.257
* **Age:** -0.065
* **SibSp:** -0.035
* **Parch:** +0.082

Passenger class had the strongest numerical correlation with survival among the variables analyzed.

The negative correlation occurs because passenger classes are represented numerically as 1st, 2nd and 3rd class. A higher numerical class value represents a lower passenger class and was associated with lower survival.

It is important to remember that **correlation does not imply causation**.

---

# Conclusion

The exploratory data analysis of the Titanic dataset revealed several important patterns in passenger survival.

The strongest patterns were associated with **gender and passenger class**. Female passengers had a substantially higher survival rate than male passengers, while passengers in higher classes generally had better survival outcomes. When gender and passenger class were analyzed together, the difference became even more evident, with 1st-class females showing the highest survival rate and 3rd-class males showing the lowest.

Fare was also positively associated with survival, which is likely connected to passenger class. Age, on the other hand, showed only a weak relationship with survival. Family-related variables showed some patterns, but their results should be interpreted carefully because some family-size categories contained relatively few passengers.

The data cleaning process successfully handled missing values in **Age** and **Embarked**, while the **Cabin** column was removed because it contained a large proportion of missing values. No duplicate records were found.

Overall, the analysis demonstrates how **data cleaning, visualization, grouping, and correlation analysis can be used to identify meaningful patterns in a dataset**. The Titanic dataset provides a clear example of how multiple variables can be explored to understand differences in outcomes.

## Skills Demonstrated

* Data Cleaning
* Handling Missing Values
* Exploratory Data Analysis (EDA)
* Pandas
* Matplotlib
* Seaborn
* GroupBy Analysis
* Data Visualization
* Correlation Analysis
* Pattern and Trend Identification

