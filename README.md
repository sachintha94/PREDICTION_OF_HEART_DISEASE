# PREDICTION_OF_HEART_DISEASE
In this project, I employ Data Mining techniques to analyze patient health data and develop a classification system that predicts the likelihood of heart disease.

## Introduction

Heart disease is one of the leading causes of death globally, emphasizing the importance of early detection and diagnosis to improve patient outcomes. In this project, we employ Data Mining techniques to analyze patient health data and develop a classification system that predicts the likelihood of heart disease. Data Mining is a systematic process of discovering meaningful patterns, correlations, and insights from large datasets, often using machine learning algorithms for prediction and decision-making.
The dataset used for this study contains 918 records and 12 attributes, representing key health indicators such as Age, Sex, ChestPainType, RestingBP, Cholesterol, MaxHR, and a target variable, HeartDisease, which indicates whether the patient has heart disease (1) or not (0). Additional features like FastingBS, RestingECG, ExerciseAngina, and ST_Slope provide further insights into patients' clinical and physical conditions.

## Dataset Attributes
  Age : age of the patient [years]
  Sex : sex of the patient [M: Male, F: Female]
  ChestPainType : chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
  RestingBP : resting blood pressure [mm Hg]
  Cholesterol : serum cholesterol [mm/dl]
  FastingBS : fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
  RestingECG : resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
  MaxHR : maximum heart rate achieved [Numeric value between 60 and 202]
  ExerciseAngina : exercise-induced angina [Y: Yes, N: No]
  Oldpeak : oldpeak = ST [Numeric value measured in depression]
  ST_Slope : the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
  HeartDisease : output class [1: heart disease, 0: Normal]

Link: https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset/data

## Design
![Capture](https://github.com/user-attachments/assets/e08d9729-9347-4c4e-9c02-d925e6b27742)

## Discussion

The primary objective of this analysis is to predict heart disease using machine learning models, evaluating their performance across two strategies: a 3% split validation and 10-fold cross-validation. Three models—Support Vector Machine (SVM), K-Nearest Neighbors (KNN), and Random Forest—were assessed based on metrics such as accuracy, precision, recall, and F1-score.
In the 3% split validation, the dataset was divided into 97% training and 3% testing data. Among the models, Random Forest achieved the highest accuracy (88.6%), precision (88.6%), recall (92.1%), and F1-score (90.3%), demonstrating its ability to effectively capture complex relationships in the data. SVM followed with balanced metrics, including an accuracy of 77.2% and an F1-score of 80.1%, indicating consistent but slightly lower performance. KNN, while achieving an accuracy of 71.9% and an F1-score of 75.2%, struggled to match the performance of the other models, likely due to its sensitivity to noise and the small test set.
In the 10-fold cross-validation, which offers a more robust evaluation by splitting the data into ten subsets, Random Forest once again outperformed the other models with a mean accuracy of 86.4% and a low standard deviation of 2.0%, signifying consistent and reliable performance across folds. SVM showed a mean accuracy of 71.8% with a standard deviation of 5.3%, slightly lower than its split validation performance, indicating sensitivity to variations in the dataset. KNN maintained similar performance with a mean accuracy of 69.8% and a standard deviation of 4.3%, confirming its limitations in handling complex patterns in the data.
Overall, Random Forest emerged as the most effective model for predicting heart disease, consistently demonstrating superior performance across both evaluation methods. Its ability to handle complex feature interactions and reduce overfitting makes it the best-suited model for this task.
While SVM provided balanced results, it fell short of Random Forest’s accuracy and consistency. KNN, being simple and sensitive to data distribution, underperformed compared to the other models. Based on these findings, Random Forest is recommended as the primary model for heart disease prediction. For future work, hyperparameter tuning, advanced feature engineering, and combining models into an ensemble could further enhance predictive performance.
Finally, I used the Random Forest model with a 3% split to implement the results in the front end, as it provided the best results for the analysis.


![image](https://github.com/user-attachments/assets/a0e71a99-9a05-492e-bdd7-0b5d0d7ec6df)

![image](https://github.com/user-attachments/assets/fce9d98b-8d06-4b28-8d50-e4f6784904ef)

