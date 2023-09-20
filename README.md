# Problem Statement
Examine the predictor variables to extract insights on their significance in predicting graduate admission likelihood and their interrelationships.

## Insights

### EDA

![03 EDA 1](https://github.com/jdeepanshu/chanceadmission/assets/6391462/b66a619f-3af6-4d07-99d6-583e99af4cae)

* Research: Around 55% students have done Research for high chance of Admission

* Most Students are admitted in University of Rating 3 and above

* SOP Ratings of 3.5 and 4 have high chance of Admission

* LOR Strength of 3 above and have high chance of Admission

![02 Ranked Heatmap](https://github.com/jdeepanshu/chanceadmission/assets/6391462/a6c3554d-ddea-4c12-8bf3-d7c7ac5ea134)

* A strong positive relationship exists between the 'Chance of Admit' and numerical variables (CGPA, GRE & TOEFL scores )

![04 EDA2](https://github.com/jdeepanshu/chanceadmission/assets/6391462/09e8b902-c2e3-42a0-855e-d3a5ae44f880)

* Also GRE Score , TOFEL Score and CGPA are highly correlated.

### Linear Regression

![06  Model Coeffecients](https://github.com/jdeepanshu/chanceadmission/assets/6391462/5fb5cbea-c7f4-497f-aef4-751577553b61)

* Analysis of model coefficients suggests that CGPA is the most influential predictor variable, while SOP and University Rating are the least significant.
  
![07 Predict Actual](https://github.com/jdeepanshu/chanceadmission/assets/6391462/cd1e3c29-6bf6-426c-9f53-4919c56728f9)

* Our Regression Models capture 83% of variance for chance of admission (Target Variable)

* Multicollinearity is present in the data.

* After eliminating collinear features, only two variables remain significant for predicting the target variable.

### Regression Assumption Tests

![12 Homoskedacis](https://github.com/jdeepanshu/chanceadmission/assets/6391462/74a9c784-5e86-44ee-97a3-bf5beafa2806)
![11 Residual](https://github.com/jdeepanshu/chanceadmission/assets/6391462/edaf39d8-5ec0-4523-a3f8-44ddcb47933c)
![13 Normallity](https://github.com/jdeepanshu/chanceadmission/assets/6391462/8ed0087b-aee2-41fd-8fc5-e940d1b63809)

* Other than multicolinearity, the predictor variables have met the conditions required for Linear Regression - mean of residuals is close to 0, linearity of variables, normality of residuals and homoscedasticity is established.


## Recommendations
* Business can improve predictions consider including work experience or internship, engagement in social causes like NGO and contributions to environmental initiatives as potential independent variables 

* These factors can indicate a candidate's responsibility and real-world impact, potentially serving as stronger indicators than Statement of Purpose (SOP), Research and Scores

