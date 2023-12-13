This is my attempt to predict the presence of a heart disease within patients from the prevalent 'Heart Failure Prediction Dataset' from Kaggle: https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction/discussion/438385

The Goal is to predict which patients suffer from 1 of 5 common cardio-vascular diseases
The data consists of a 12X918 with the following features (From the original file description):

1) Age: age of the patient [years]

2) Sex: sex of the patient [M: Male, F: Female]

3) ChestPainType: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]

4) RestingBP: resting blood pressure [mm Hg]

5) Cholesterol: serum cholesterol [mm/dl]

6) FastingBS: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]

7) RestingECG: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]

8) MaxHR: maximum heart rate achieved [Numeric value between 60 and 202]

9) ExerciseAngina: exercise-induced angina [Y: Yes, N: No]

10) Oldpeak: oldpeak = ST [Numeric value measured in depression]

11) ST_Slope: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]

12) HeartDisease: output class [1: heart disease, 0: Normal]


The code consists of the entire research process - from initial data comprehension, through experimental naive runs, through extensive GridSearch and ends with attempt at dimention reduction
using the best found model.

Since this was a concluding project for my studies at John Bryce, I attempted every algorithm I was aware of - even ones that seemed useless for a categorization problem like this one,
such as Linear Reg model.

I managed to arrive at a recall score of 91% and an f1 score of 92% with Soft Voting model composed of the best found models of: Logistic Reg, Decision Tree, Random Forest, SVC, KNN and XGBoost.
All models were Grid Searched for the best performing parameters, and were used for Voting with those parameters.

Further insights can be found at the 'Summery' file.
