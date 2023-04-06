# Group-Project - Heart Disease Prediction
https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data 


Goal: Select 3 classifier that best correlates with the characterization of heart disease and use these classifiers to build a classification model to predict whether a new patient is likely to have heart disease. 


RQ: which three predictors best correlates with the characterization of heart disease and can these predictors be used to build an accurate classification model to predict whether a new patient is likely to have heart disease?
![image](https://user-images.githubusercontent.com/124746271/230509337-59438029-995c-4c75-8651-de3fd6df06f5.png)



Proposal feedback
- The proposal seems to lack a specific research question or hypothesis that the project aims to solve. Age, Cholesterol, Blood Pressure Levels are three random health indicator. When it is a project question you should find a more general question to solve like " Heart diseases identification using the most significant heart health indicators" - For EDA a summary of statistics would be helpful. - Nothing about modeling methods was mentioned, including test-train splitting, data preprocessing, selection of k using cross-validation, or evaluating the prediction. - Results statements are general, and any specific steps to achieve these goals have not been provided. - You should specify the outcomes rather than make general statements.


# Introduction
Heart disease has been the leading cause of death in the United States since 1950. The term heart disease describes a range of conditions that could affect the heart. The most common heart diseases are coronary heart disease, peripheral artery disease, and aortic disease. Studies show that the leading risk factors for these diseases include high blood pressure and cholesterol. Specific medical conditions like unhealthy diets, physical inactivity, and smoking tend to put an individual at a higher risk. We aim to develop an accurate model to predict whether an individual has heart disease based on their cholesterol levels, heart rate and age. To approach this question, we will use three predictor values, heart rate, cholesterol levels, and age, from the heart data set containing 76 attributes. Hence, we would classify an individual as either positive or negative for Heart Disease.

# Methods
(old)Methods:

After we understand the dataset through exploratory data analysis and data preparation, we will aim to build diagnostic prediction models with a binary outcome. The heart disease database contains 76 attributes, however, the data set loaded for this project only includes 14 attributes. All of which, a single observation in the dataset represents an individual's health records, including their age, sex, chest pain type, resting blood pressure, cholesterol, fasting blood sugar, resting electrocardiography, max heart rate achieved, exercise, old peak, the slope of peak exercise, number of major vessels, and diagnosis status.

Our models will only use three variables/columns: the person's age, cholesterol levels, and maximum heart rate. For our visualization, we will be using scatterplots to visually check if there exist some relation between numeric variables. Since scatter plots are dispersion graphs built to represent the data points of variables, we believe this will be an effective way to visualize and predict values. Histograms will also be used to observe the distribution of different attributes.

In our project, we will only plot the attributes relevant to our analysis: age, cholesterol, and maximum heart rate. Using histogram data makes it easy for us to identify that the three attributes are categorical, as if they were not, there would be significant gaps between each bar.

Addtionally, we value the room for errors data by checking for missing data. The process revolves around inspecting each and single dataframe and check for non numerical values that do not fit into our goal of data analysis. This process can be complex as the data that we inspect do not measure missing data as "NA", but rather "?", such that the functions to detect NAs such as "is.na" could not be used. As such, the method used to filter for "?" in our data is to isolate each variable and look for "?". As a result, we found "?" in the "age", "cholesterol" and "thalach" columns, which does not affect the variables that we are interested in.

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

This project uses data from the Cleveland Clinic Foundation retreived from https://archive.ics.uci.edu/ml/datasets/Heart+Disease. 

the predicted attribte is the "num" column which indicates the diagnosis of heart disease. According to the data description, a value of 0 means not likely to have heart disease; any value that is not 0 means patient is likely to have heart disease. To change the predicted attribute to be catagorical, the ifelse function was used to convert any non-zero numbers to 1. The final result of the prediction is now either 0 (not likely to have heart disease) or 1 (likely to have heart disease). 
