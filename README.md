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

*Machine Learning Comparisons*
- Random Forest suggests that numeric variables with relatively high correlation with attrition are useful in predicting attrition
- Logistic Regression is not recommended as a technique as most categorical variables are irrelevant in determining attrition
- Neural Network is highly useful in effectively predicting attrition

*Data Driven Insights*
- Common profile of employees who quit: low salary, lives far away from office, low chance of career progression/lack of opportunities
- Actions for IBM: increase salary incentives, enhance effective employee assessments, change up roles in senior management

### What we have learnt from this project?
- Using pandas.get_dummies to convert catrgorical variables into indicator variables
- Logistic Regression model 
- Justify the suitability of a model based on readings from classification report
- Neural Network model

### References
1. https://analyticsindiamag.com/guide-to-hyperparameters-tuning-using-gridsearchcv-and-randomizedsearchcv/
2. https://www.analyticsvidhya.com/blog/2021/06/understanding-random-forest/
3. https://stackoverflow.com/questions/55229301/one-hot-encoding-multiple-columns-in-sklearn-and-naming-columns
4. https://www.datacamp.com/community/tutorials/understanding-logistic-regression-python
5. https://towardsdatascience.com/building-a-logistic-regression-in-python-step-by-step-becd4d56c9c8
6. https://github.com/PacktPublishing/Deep-learning-with-PyTorch-video
7. https://androidkt.com/load-pandas-dataframe-using-dataset-and-dataloader-in-pytorch/
