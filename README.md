# Exploratory-Data-Analysis-EDA-Phyton
The visual study demonstrates that fare, class, and gender all had a significant impact on survival on the Titanic, with females and first-class passengers having the highest survival percentages.  Passengers with children and higher incomes had a higher chance of surviving, but age alone was less important.
## Data Used
- <a href="https://github.com/nimmagantiharini/Exploratory-Data-Analysis-EDA-Phyton/blob/main/gender%20file%20titanic%201.csv"> Raw Dataset of Gender</a>
- <a href="https://github.com/nimmagantiharini/Exploratory-Data-Analysis-EDA-Phyton/blob/main/Train%20file%20titanic%203.csv"> Raw Dataset of Train</a>
- <a href="https://github.com/nimmagantiharini/Exploratory-Data-Analysis-EDA-Phyton/blob/main/Test%20file%20titanic%202.csv"> Raw Dataset of Test</a>
## Install Dependencies
import pandas as pd  
import matplotlib.pyplot as plt
import seaborn as sns
## Output:
- <a href="https://github.com/nimmagantiharini/Exploratory-Data-Analysis-EDA-Phyton/blob/main/TITANIC%20PDF.pdf"> Observations PDF </a>
- - <a href="https://github.com/nimmagantiharini/Exploratory-Data-Analysis-EDA-Phyton/blob/main/Titanic1-Copy1.ipynb"> Titanic Phyton file</a>
## overall insights
Survival was not random. It depended heavily on gender, class, age, and wealth. The strongest trends:
•	Females > Males
•	1st Class > 2nd > 3rd
•	Children > Adults > Elderly
•	Wealthier passengers (high fare) > Poorer passengers (low fare)
## Relationship and Trends
1.Gender & Survival
-Women survived far more than men.
-This reflects the “women and children first” rule.
2.Class (Pclass) & Survival
-1st Class passengers had the highest survival rate.
-3rd Class passengers had the lowest survival rate.
-Strong negative correlation between Pclass and survival.
3.Fare & Survival
-Higher fares → higher survival probability.
-Suggests that wealthier passengers had better access to lifeboats (linked to class).
4.Age & Survival
-Children (≤10 years) had a higher chance of survival.
-Older passengers had lower survival rates.
5.Family Size (SibSp + Parch) & Survival
-Small families (1–2 relatives) had better survival.
-Very large families had low survival chances.
-Single passengers also had lower survival compared to small families.
6.Embarked Port & Survival
-Passengers from Cherbourg (C) had a higher survival rate compared to Southampton (S).
7.Correlation Trends (from heatmap)
-Survived positively correlates with Fare, negatively with Pclass.
-Pclass is strongly tied to Fare (wealthy passengers traveled in 1st class).
-SibSp and Parch are moderately correlated → families traveling together.
## Observation of Each Visual
# 1.Count plot:
A. 
- The plot shows two bars: 0 = Did Not Survive, 1 = Survived.
 -The “0” bar (non-survivors) is much taller than the “1” bar (survivors).
 -This means the majority of passengers did not survive the Titanic disaster.
 -The dataset survival rate is about 38% survived vs 62% did not survive.
B.First-class passengers had the highest survival rate, second-class had moderate survival, while third-class faced the lowest chances. This shows that socioeconomic status played a major role in survival on the Titanic.
# 2.Histoplot:
 -Most passengers were between 20–40 years old.
 -Fewer children and elderly passengers.
  -Right-skew shows fewer older individuals (>60).
# 3.pairplot
•	Age vs Survival
Survivors are slightly younger on average.
Children (<10 years old) show higher survival.
•	Fare vs Survival
Survivors often paid higher fares (linked to 1st class).
Many low-fare passengers did not survive.
•	Pclass vs Survival
Strong split: 1st class passengers had much higher survival.
3rd class dominated by non-survivors.
•	SibSp / Parch vs Survival
Small families (1–2 relatives) had better survival chances.
Very large families had lower survival.
# 4.Heatmap
Fare has a positive correlation with survival (~0.26) → higher fares = better chance.
Pclass has a negative correlation (~ -0.34) → higher class number (3rd) = lower survival.
Age correlation with survival is weak (~ -0.08).
SibSp and Parch show weak correlations, but families of size 1–2 had better chances than singles or very large families.
# 5.Histoplot:
Most fares are low (<100), but there are outliers with very high fares.
# 6.box plot:
1st class fares are much higher on average compared to 2nd and 3rd.
# 7.scatter plot:
Survivors tend to cluster at younger ages and higher fares.
# 8.stripplot:
The stripplot shows that females across most ages had higher survival, while many males, especially adults, did not survive. This clearly reflects the “women and children first” evacuation pattern on the Titanic.

## SUMMARY OF FINDINGS:
	In total, a greater number of passengers perished than survived.
	The fact that females lived longer than males indicates that gender had a significant impact on survival.
	Passengers in first class had the highest survival rate, while those in third class had the lowest.
	Higher fares were linked to better survival chances.
	Younger people and children, particularly girls, fared better in terms of survivability.
	Cherbourg (C) passengers fared better than Southampton (S) and Queenstown (Q) passengers.
	A heatmap and pairplot demonstrated that, although age alone had less of an impact, survival had a positive correlation with fare and class.





