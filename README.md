# SC1015 Mini-Project
## About
For our mini project in the Introduction to Data Science and Artificial Intelligence module (SC1015), we performed analysis on Mitchell Gleason's Formula 1 [dataset](https://github.com/MitchellGleason/F1-Data-Analysis--Wet-Races) from GitHub, supplemented with race data from the most recent [Singapore 2023 Grand Prix](https://www.formula1.com/en/results.html/2023/team.html) as it was missing

## Problem Definition
- What should teams work towards to improve their standings?
- How can we utilise machine learning to accurately predict the top 5 drivers given factors of a race?
- Narrowed down to the Singapore Grand Prix given that variables such as race duration, laptimes and track mileage differ from country to country. 

## Contributors
FCEA - Team 8
1. Isaac Leow - Contribution
2. Tan Jun Wei Adison - Contribution
3. Goh Jin Long Abdillah - Contribution

## Files Included
1. Datasets
    - laptimesgit.csv
    - qualifyinggit.csv
    - racesgit.csv
    - sgppitsgitfinal.csv
    - resultsgit.csv
    - weatherdescriptiongit.csv
2. SC1015 Mini-Project Slides.pdf - presentation slides used
3. SC1015 Final Formula 1 Mini-Project
    - Initial Data Insights
    - Data Preparation & Cleaning
    - Exploratory Data Analysis
    - Machine Learning


## Notebook Details
### Initial Data Insights
   a. Extracting the Singapore Grand Prix Data from the datasets

   b. Check for suitable values to use as prediction variables

   
   
### Data Preparation & Cleaning
   a. Remove insignificant columns: 'EmployeeCount', 'Over18', 'StandardHours', and 'EmployeeNumber'

   b. Merge all datasets together and dropped NULL values

   c. Changed response variable to 0/1, to indicate Top5/NotTop5 and enhanced readability of variable names



### Exploratory Data Analysis
   a. Uni-variate Statistics to get a sense of the values we are working with

   b. Bi-variate relationships between predictors and response variables

   c. Multi-variate Statistics to see prediction variables and their correlation to each other



### Machine Learning
*1. Classification Tree*

*2. Support Vector Machine (SVM)*

*3. Logistic Regression*

*4. Random Forest*

*5. Hyperparameter Tuning of SVM, Logistic Regression and Random Forest using GridSearchCV*


## Conclusion

- We are able to determine whether a driver would end up in the Top 5 with relatively high accuracy in the context of Singapore using Machine Learning Models
- However, some variables are hard to obtain when spectating a race in real time for fans who wish to predict the top 5, but the grid / starting positions of the drivers can be quite a suitable and reliable starting indicator of whether the driver would end up in the top 5. From there, as the race moves forward, we are able to input the rest of the variables to better increase our prediction accuracy.
- SVM and Logistic Regression could not perform as well as Random Forest, even with the hyperparameters tuned
- Actions for F1 teams: Teams and drivers need to commit fully during qualifiers, hire better drivers and have more practice to improve their consistency, have more investment into R&D and increase amount of pit stop practices and employ better strategies


## What we have learnt from this project?
- Logistic Regression, SVM and Random Forest machine learning models
- Hypertuning our parameters using GridSearchCV

### References
1. https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_val_score.html
2. https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
3. https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
4. https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html
5. https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html
6. https://scikit-learn.org/stable/modules/model_evaluation.html
