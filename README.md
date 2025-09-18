# Titanic_1 Summary Report


 Titanic Survival Prediction using Random Forest
This project implements a Random Forest classifier  to predict the survival of passengers from the Titanic disaster. The model is built using only basic Python, pandas, and numpy, without using scikit-learn's built-in RandomForestClassifier

 Key Findings and Insights

- Who survived?  
  - Women and children had a much higher survival rate than men and adults.
  - 1st class passengers survived more often than 2nd or 3rd class.
  - Higher fare and having a cabin (not missing) were linked to higher survival.
  - Family size and passenger title (Mr, Mrs, Miss, etc.) also helped predict survival.

- **Most important features :
  - Sex (being female increased survival odds)
  - Pclass (1st class was safer)
  - Title (Miss, Mrs, Master, etc.)
  - AgeBin (younger passengers survived more)
  - FareBin (higher fare, higher survival)
  - FamilySize (traveling with family helped a bit)


Model Performance Summary

- Validation Accuracy: 0.8156424581005587 
Confusion Matrix:
 [[92 13] [20 54]]
-Precision: 0.8059701492537313
-Recall: 0.7297297297297297
-F1 Score: 0.7659574468085106
________________________________________



Feature Importances:
 {'FamilySize': 0.11791383219954649,
 'Sex': 0.06575963718820861, 
'HasCabin': 0.07256235827664399,
 'FareBin': 0.12471655328798185,
 'Pclass': 0.12471655328798185, 
'AgeBin': 0.10884353741496598,
 'Title': 0.11337868480725624,
 'Embarked_S': 0.05668934240362812, 
'SibSp': 0.09297052154195011,
 'Parch': 0.08616780045351474,
 'Embarked_Q': 0.036281179138321996}
 
 Challenges Faced and Solutions

Building the tree recursively:
  I found recursion a bit confusing at first
Handling missing and categorical data and figuring out how to fill missing values and convert categories to numbers was tricky. 

--Future Improvement Suggestions
Use Advanced Libraries:
  If allowed, using libraries like scikit-learn would make the code much faster, more reliable, and easier to tune. Their RandomForestClassifier is highly optimized and has many extra features.
Try More Models:
  Experiment with other machine learning models like Gradient Boosting, XGBoost, or even neural networks to see if they improve accuracy and precision.
- Handle Missing Data Better:  
  Use more advanced imputation methods (like KNN imputation or regression imputation) instead of just filling with median or mode.


---


