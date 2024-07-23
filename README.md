

# Predicting the Survival of Patients with Heart Failure

Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year. CVDs are a group of disorders of the heart and blood vessels and include coronary heart disease, cerebrovascular disease, rheumatic heart disease and other conditions. Four out of 5CVD deaths are due to heart attacks and strokes, and one third of these deaths occur prematurely in people under 70 years of age.
Most cardiovascular diseases can be prevented by addressing behavioural risk factors such as tobacco use, unhealthy diet and obesity, physical inactivity and harmful use of alcohol using population-wide strategies.



<p align="center">
<img src="https://americanaddictioncenters.org/wp-content/uploads/2016/06/heart-icon.png" width="250" height="250" />
</p>
Individuals at risk of CVD may demonstrate raised blood pressure, glucose, and lipids as well as overweight and obesity. These can all be easily measured in primary care facilities. Identifying those at highest risk of CVDs and ensuring they receive appropriate treatment can prevent premature deaths. Access to essential noncommunicable disease medicines and basic health technologies in all primary health care facilities is essential to ensure that those in need receive treatment and counselling.

# Dataset
The dataset contains medical records of 299 patients who had heart failure, collected during their follow-up period, where each patient profile has 13 clinical features. https://archive.ics.uci.edu/ml/datasets/Heart+failure+clinical+records

### Attributes information:
![](https://i.imgur.com/niqOo77.png)

### Experiment Results:
* **Data Analysis**
    * 5 columns contains outliers this columns are ( creatitinine_phosphokinase, ejection_fraction, platelets, sereum_creatinine, serum_soidum).
    * Imbalanced target class ( I'll used resampling techniques to add more copies of the minority class )
 * **Performance Evaluation**
    * Splitting the dataset by 80 % for training set and 20 % validation set.
 * **Training and Validation**
    * After training and experimenting different algorithms using ensemble models have good accuracy score than linear and nonlinear models.
    * Gradient Boosting Classifier ( 93 % accuracy score )
 * **Fine Tuning**
    * Using {'learning_rate': 0.1, 'max_depth': 9, 'n_estimators': 1000, 'subsample': 0.7} for Gradient Boosting Classifier improved the accuracy by 1 %.
 * **Performance Results**
    * Validation Score: 97%
    * ROC_AUC Score: 96.9 %
 


![](https://i.imgur.com/Yrn231v.png)

## Project Scope and Objective

A heart failure recognition project aims to develop a system or model capable of accurately identifying individuals at risk of or experiencing heart failure. This can be achieved through various approaches, including:

Early detection: Identifying individuals at high risk of developing heart failure based on clinical data and lifestyle factors.
Diagnosis support: Assisting healthcare professionals in diagnosing heart failure by analyzing medical images, electrocardiograms (ECGs), or other relevant data.
Prognosis prediction: Estimating the progression of heart failure and predicting patient outcomes.


## Methodology
The project typically involves the following steps:

Data collection and preprocessing: Gathering relevant data, cleaning, and formatting it for analysis.
Feature engineering: Extracting meaningful features from raw data, such as heart rate variability, blood pressure patterns, or image-based features.
Model development: Selecting and training appropriate machine learning or deep learning algorithms (e.g., random forest, support vector machines, convolutional neural networks).
Model evaluation: Assessing the performance of the model using metrics like accuracy, sensitivity, specificity, and precision.
Model deployment: Integrating the model into a clinical workflow or developing a user-friendly application.


## Potential Challenges and Considerations

Data quality: Ensuring data accuracy, completeness, and consistency is crucial.
Imbalanced data: Heart failure is often a rare condition, leading to imbalanced datasets. Addressing this requires techniques like oversampling or undersampling.
Ethical considerations: Protecting patient privacy and ensuring data security is paramount.
Clinical validation: Thoroughly validating the model in a clinical setting is essential before widespread adoption.


## Additional Considerations
Explainability: Understanding how the model arrives at its predictions is crucial for building trust and ensuring ethical use.
Continuous learning: The model should be able to learn from new data and improve over time.
Integration with electronic health records (EHRs): Seamless integration can facilitate data access and clinical workflow.

