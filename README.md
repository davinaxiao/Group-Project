# Group-Project - Heart Disease Prediction
https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data 

Heart disease has been the leading cause of death in the United States since 1950. The term heart disease describes a range of conditions that could affect the heart. The most common heart diseases are coronary heart disease, peripheral artery disease, and aortic disease. Studies show that the leading risk factors for these diseases include high blood pressure and cholesterol. Specific medical conditions like unhealthy diets, physical inactivity, and smoking tend to put an individual at a higher risk. Using this dataset, we hope to develop an accurate model to predict whether an individual has heart disease and which specific factors have led to the cause. To approach this question, we plan to use different classification methods, and algorithms...

#Data Set Information:

This database contains 76 attributes, but all published experiments refer to using a subset of 14 of them. In particular, the Cleveland database is the only one that has been used by ML researchers to
this date. The "goal" field refers to the presence of heart disease in the patient. It is integer valued from 0 (no presence) to 4. Experiments with the Cleveland database have concentrated on simply attempting to distinguish presence (values 1,2,3,4) from absence (value 0).

The names and social security numbers of the patients were recently removed from the database, replaced with dummy values.

One file has been "processed", that one containing the Cleveland database. All four unprocessed files also exist in this directory.

To see Test Costs (donated by Peter Turney), please see the folder "Costs"

#Features & Predictor:

Only 14 attributes used:
1. age: age of the patient(years)
2. sex: sex of the patient(M: Male,  F: Female)
3. cp: chest pain type(TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic)
4. trestbps: resting blood pressure(#)
5. chol: serum cholesterol in mg/dl(#)
6. fbs: fasting blood sugar > 120 mg/dl(Binary)(1=true; 0=false)
7. restecg: resting electrocardiography results(values 0,1,2)
8. thalach: maximum heart rate achieved (#)
9. exang: exercise induced angina (binary) (1 = yes; 0 = no)
10. oldpeak: oldpeak = ST (Numeric value measured in depression)
11. slope: of the peak exercise ST segment (Ordinal)(Value 1: up sloping , Value 2: flat , Value 3: down sloping)
12. ca: number of major vessels (0–3, Ordinal) colored by fluoroscopy
13. thal: maximum heart rate achieved — (Ordinal): 3 = normal; 6 = fixed defect; 7 = reversible defect
14. num (the predicted attribute)
