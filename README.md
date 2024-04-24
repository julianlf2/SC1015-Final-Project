# SC1015 Mini-Project
## About
For our mini project in the Introduction to Data Science and Artificial Intelligence module (SC1015), we performed analysis on [Mitchell Gleason's Formula 1 dataset](https://github.com/MitchellGleason/F1-Data-Analysis--Wet-Races) from GitHub, supplemented with race data from the most recent [Singapore 2023 Grand Prix](https://www.formula1.com/en/results.html/2023/team.html) as it was missing.

## Problem Definition
- What should teams work towards to improve their standings?
- How can we utilise machine learning to accurately predict the top 5 drivers given factors of a race?
- Narrowed down to the Singapore Grand Prix given that variables such as race duration, laptimes and track mileage differ from country to country. 

## Contributors
FCEA - Team 8
1. Isaac Leow - EDA, SVM, Logistic Regression, Script Preparation, GridSearchCV (for SVM, RandomForest, Logistic Regression)
2. Tan Jun Wei Adison - Data Preparation and Cleaning, EDA, Decision Tree, RandomForest, Script Preparation
3. Goh Jin Long Abdillah - Data Preparation and Cleaning, Logistic Regression, Slides Preparation, Video, Script Preparation

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

## Slides Details
Our slides highlight the intricacies of crucial information and relationships found during our exploration in the Python Notebook. It considers the most raw form of our data and how we transformed it into an eventual prediction model through data cleaning, exploratory data analysis and exploration of machine learning models to draw logical conclusions and predictions.

## Notebook Details
### Initial Data Insights
   a. Extracting the Singapore Grand Prix Data from the datasets

   b. Check for suitable values to use as prediction variables

   
   
### Data Preparation & Cleaning
   a. Utilised pre-requisite Python coding knowledge together with large datasets to perform feature engineering and better exploration of given problems. 

   b. Merge all datasets together and study contextual information before dropping information such as NULL values and points earned.

   c. Changed response variable to 0/1, to indicate Top5/NotTop5 and improve readability of dataframe through Ids such as years and drivers.



### Exploratory Data Analysis
   a. Use of a variety of plots for Uni-variate Statistics to better visualise and understand the individual variables and their complexities we are working with.

   b. Explore Bi-variate relationships between predictors and response variables to infer what other crucial information can be extracted for machine learning usage.

   c. Perform Multi-variate Statistics Visualization to study the interplay between predictors and how this effects the response variable.



### Machine Learning
*1. Classification Tree*

*2. Support Vector Machine (SVM)*

*3. Logistic Regression*

*4. Random Forest*

*5. Hyperparameter Tuning of SVM, Logistic Regression and Random Forest using GridSearchCV*


## Conclusion

- We are able to determine whether a driver would end up in the Top 5 with relatively high accuracy in the context of Singapore using Machine Learning Models.
- Teams can utilise the same approach in different countries. While the accuracy of the models might differ, overall, the model should still prove effective in predicting the Top 5.
- However, some variables are challenging to obtain when spectating a race in real time for fans and teams who wish to predict the top 5. The variable starting grid positions of the drivers can however be quite a suitable and reliable indicator, available before races, helping us predict whether the driver would end up in the top 5. From there, as the race moves forward, we are able to input the real time race variables to better increase our prediction accuracy. Teams can utilise this information to help them make better decisions mid-race, improving their chances of top positions.
- SVM and Logistic Regression could not perform as well as Random Forest, even with the hyperparameters tuned. Ultimately, Random Forest together with GridSearchCV procured the best prediction model.
- Actions for F1 teams: Teams and drivers need to commit fully during qualifying to secure good starting grid spots. Employ better drivers and have practice more to improve their consistency. Direct more investments into R&D to build a better car. Increase frequency of pit stop practices and employ better pitting strategies such as an undercut.


## What we have learnt from this project?
- Support Vector Machines and SVM kernels
- Logistic Regression and their folds
- Random Forest Search
- Hypertuning machine learning model parameters using GridSearchCV
- Precision, Recall, F1 score
- Upsampling, Random sampling and One-Hot Encoding. (One-Hot Encoding was removed from the notebook as we realised that it caused the classification accuracy of the machine learning models to drop)

### References
1. https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_val_score.html
2. https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
3. https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
4. https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html
5. https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html
6. https://scikit-learn.org/stable/modules/model_evaluation.html
7. https://en.as.com/racing/how-much-revenue-was-generated-by-f1-during-the-2023-season-n/
8. https://www.todayonline.com/big-read/big-read-singapore-goes-all-f1-will-it-pay-desperate-tourism-sector-1809766
9. https://www.forbes.com/sites/bradadgate/2024/03/11/heres-why-formula-1-racing-is-growing-in-popularity-with-women/?sh=253f316d137c
10. https://www.the-race.com/formula-1/f1-2024-teams-entry-fees/
