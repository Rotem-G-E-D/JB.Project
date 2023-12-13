This is my attempt to predict the presence of a heart disease within patients from the prevalent 'Heart Failure Prediction Dataset' from Kaggle: https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction/discussion/438385

The Goal is to predict which patients suffer from 1 of 5 common cardio-vascular diseases
The data consists of a 12X918 with the following features:

Age: Age of patient at checkup (years). [Numeric]
Sex: Either Male or Female. [Categorical – M/F]
Chest Pain Type: Type of chest pain reported by the patient. [Categorical – 4 types]
Max HR: Maximum Heart-Rate reached during exercise (bpm). [Numeric]
Exercise Angina: Chest pain during exercise. [Categorical – Yes/No]
ST Slope: The slope of a particular area in the wave form of a heartbeat ECG during exercise. Correlates to different types of coronary artery problems. [Categorical – 3 types]

The code consists of the entire research process - from initial data comprehension, through experimental naive runs, through extensive GridSearch and ends with attempt at dimention reduction
using the best found model.

Since this was a concluding project for my studies at John Bryce, I attempted every algorithm I was aware of - even ones that seemed useless for a categorization problem like this one,
such as Linear Reg model.

I managed to arrive at a recall score of 91% and an f1 score of 92% with Soft Voting model composed of the best found models of: Logistic Reg, Decision Tree, Random Forest, SVC, KNN and XGBoost.
All models were Grid Searched for the best performing parameters, and were used for Voting with those parameters.

Further insights can be found at the 'Summery' file.
