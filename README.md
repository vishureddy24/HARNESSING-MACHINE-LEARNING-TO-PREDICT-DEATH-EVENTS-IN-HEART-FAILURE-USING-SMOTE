# HARNESSING-MACHINE-LEARNING-TO-PREDICT-DEATH-EVENTS-IN-HEART-FAILURE-USING-SMOTE
Project Overview
Heart disease is one of the leading causes of mortality in the world, and heart failure is a severe condition that has a significant impact on patient survival. Early prediction of heart failure outcomes can help healthcare professionals improve patient management and reduce mortality rates. However, predicting death events in heart failure patients is challenging due to the complexity of clinical data and the imbalance in datasets, where death events are relatively rare compared to survival cases.

This project investigates the use of machine learning techniques for the prediction of death events in heart failure patients. It specifically deals with class imbalance using the Synthetic Minority Over-sampling Technique (SMOTE) and compares different machine learning algorithms to come up with a strong predictive model. In India, alone, it accounts for a huge percentage of deaths, which has multiple risk factors like hypertension, diabetes, and high cholesterol. Traditional statistical models have been used for the purpose of risk prediction, but they often do not work with complex relationships in clinical data. Machine learning can provide an alternative approach that may analyze large datasets and uncover hidden patterns, thereby giving more accurate and efficient models for prediction. However, one of the biggest challenges in training predictive models for heart failure mortality is the imbalance in datasets. Because fewer patients die than survive, models tend to be biased towards the majority class, which would lead to poor sensitivity in death event prediction. SMOTE helps in balancing the dataset by generating synthetic samples for the minority class so that the model generalizes well.

The key aims of this work are:  
1. Create predictive models that can classify the heart failure patient in terms of survival outcomes 
2. Improve the performance by dealing with the class imbalance issues using SMOTE
3. Compare multiple algorithms for machine learning and compare those for their predicting ability in events of death  
4. Explore key clinical features in heart failure prognosis.
5. A decision-support system** to support healthcare professionals in the effective management of high-risk patients.  
------------------------------------------------

Methodology

1. Data Collection & Preprocessing 

The dataset for this research is comprised of medical records of **299 heart failure patients** from Allied Hospital and the Faisalabad Institute of Cardiology, Pakistan. It comprises 13 clinical features, including: 
- Age 
- Sex 
- Smoking status 
- Ejection fraction
- Seruma creatinine
 - Hypertension
 - Diabetes
 - Platelet count
 - Serum sodium
 - Anemia
The data was cleaned, the missing values were imputed, and then the dataset split into sets while using training and testing to evaluate the model. 

2. Class Imbalance Handling

Dealing with the class imbalance (203 survived, 96 died), SMOTE was applied to over-sample the minority class (death events). This guaranteed that the data received by machine learning models would be balanced; hence, a better performance is expected for the prediction of rare events. 
3. Machine Learning Models 

Nine machine learning models were implemented and compared regarding their performance. These include:
- Decision Tree (DT)
- Adaptive Boosting (AdaBoost)
- Logistic Regression (LR)
- K-Nearest Neighbors (KNN) 
- Random Forest (RF)
- Gradient Boosting Classifier (GBM)  
- Extra Trees Classifier (ETC) 
- Gaussian Naive Bayes (GNB)  
- Support Vector Machine (SVM)  
Each model was trained and tested with a set of performance metrics to identify the top-performing model for heart failure mortality prediction.  

4. Performance Evaluation

Because the classes are imbalanced, just standard accuracy alone was not suitable for the metric. The models were judged based on the following performance metrics.
 Receiver Operating Characteristic (ROC) and Area Under the Curve (AUC)
Accuracy
Sensitivity or Recall – measures how good is the model at detecting an actual death event. 
Matthews Correlation Coefficient (MCC) – ensures proper balancing of metrics for datasets that are imbalanced. 
--- 
Results & Discussion

Feature analysis showed that **ejection fraction and serum creatinine levels were the most significant predictors of heart failure mortality. Patients who had lower ejection fractions and higher levels of serum creatinine exhibited a significantly increased risk of death.  The **visualization through scatter plots showed that the elders had lower platelet counts and higher mortality. The SMOTE-enhanced models were better than the conventional models in terms of identifying high-risk patients with excellent precision.

Among all models, Random Forest and Gradient Boosting** performed the best in terms of overall performance, giving a high AUC score, strong recall, and balanced precision.

This shows that the integration of machine learning with SMOTE improves much on the heart failure death event prediction. The proposed models may be applied as useful decision-support tools to healthcare professionals in early identification of high-risk patients and taking preventive measures.  Future work** can be:  

- More patients from other demographics should be included in the dataset.  - Deep learning techniques for better accuracy can be considered.
- Consolidation of time-series data to monitor the patient's health over time. 
- Creating an intuitive web application** to present the predictions to both doctors and patients. 
With the power of machine learning, this work opens avenues for **enhanced clinical decision-making and patient outcomes in the management of heart failure. 

---

