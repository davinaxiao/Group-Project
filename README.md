# Group-Project - Heart Disease Prediction
https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data 

# Introduction
Heart disease has been the leading cause of death in the United States since 1950. The term heart disease describes a range of conditions that could affect the heart. The most common heart diseases are coronary heart disease, peripheral artery disease, and aortic disease. Studies show that the leading risk factors for these diseases include high blood pressure and cholesterol. Specific medical conditions like unhealthy diets, physical inactivity, and smoking tend to put an individual at a higher risk. We aim to develop an accurate model to predict whether an individual has heart disease based on their cholesterol levels, heart rate and age. To approach this question, we will use three predictor values, heart rate, cholesterol levels, and age, from the heart data set containing 76 attributes. Hence, we would classify an individual as either positive or negative for Heart Disease.

# Methods

# Expected outcomes and significance:
What do you expect to find?
What impact could such findings have?
What future questions could this lead to?

We expect that patients with high cholesterol and blood pressure levels are more likely to have heart disease than those with lower levels. We believe that age will also significantly affect our results as health issues are more common in older adults. This leads us to...

# Features & Predictor:
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