# MIMIC_II_Database_Analysis
Analysis and Disease Prediction Using MIMIC II Database

# Objective
By analyzing ICU Admitted Patients’ Data (MIMIC II), here we tried to build up a Machine Learning model which can efficiently and correctly classify the category of the disease in the patient based on its vital signs, age and gender, even before the patient reaches the hospital. So that the arrangements for his treatment can be made readily, consequently saving lives due to this early diagnosis of the disease.


# Methodology

## Data Gathering:

By analyzing ICU Admitted Patients’ Data, here we tried to build up a Machine Learning model which can efficiently and correctly classify the disease of the patient based on its vital signs, age and gender, even before the patient reaches the hospital. So that the arrangements for his treatment can be made readily, consequently saving lives due to this early diagnosis of the disease.


## Data Understanding:

A user guide is also provided along with the MIMIC II dataset. It helps understand the collection of data, commonly used terminologies, database structure and also a demo of how to query data. 


## Preprocessing:

We had to bring the vital signs, gender, age and disease of the patient in one table. We used pandas, numpy, os and other libraries to filter, merge and save data.


## Exploratory Data Analysis:

Exploration of Data, to a great extent was carried out for determining the demographics of the patients as well as the vital signs recorded of the patients. Since we mainly had categorical data, we created several visualizations such as bar graphs and pie charts, to quickly grasp the knowledge and understanding of what kind of parameters are significant, which are the most occurring and leading ones etc. 


## Feature Engineering:

Afte compiling the vital signs, gender, age and diseases of the patients from numerous tables, we had to deal with null values, missing data and imbalanced classes of the diseases. First, we filtered out the top 10 diseases for which the patients were admitted to the hospital. Then the null and missing values in vital signs were imputed with the mean of the respective types. Since there was a huge imbalance in the classes of the data. We used scikit learn’s imbalance library to Up-sample those classes, all to the same number of observations.


## Model Training and Testing:

First the dataset was spilt into train and test sets. The train set was further split into train and validation set. Various classification algorithms were validated on the training set including Logistic Regression, Decision Trees, K-Nearest Neighbors, Support Vector Machines, Random Forest etc. 
Random Forest gave the best results and therefor tested on the held-out (test set).


## Model Evaluation:

After the testing of the Random Forest, it was evaluated based on certain classification metrics including accuracy, precision, recall, F1 score and confusion matrix.


## ML Results:

Random Forest performed best among rest of the classification algorithms. We were able to reduce overfitting of the Random Forest by 24% (as compared to the original dataset). The test accuracy of the model became 81% which was 64% previously.


![ML_results_on_Synthetic_data](https://user-images.githubusercontent.com/96207722/219608406-f9151498-a547-4394-b379-62f746b48913.jpeg)



# Workflow

![Methodology_Flow_Chart](https://user-images.githubusercontent.com/96207722/219607830-5fea98e5-e53c-4526-a131-b816695d09ef.JPG)




# Conclusion

In this Research we analyzed ICU admitted data of patients of an American Hospital. We were able to identify a novel approach to utilize AI by creating an ML model which can help predict patients’ diagnosis based on providing data of gender, age and vital signs. This early detection of the disease will help reduce burden on the healthcare force. They could now be more alarmed and prepared to treat the patient based on the fact that they have certainty of patients’ disease. This will be helpful as they could arrange the treatment and medical tests for the patient based on the diagnosis beforehand. This would staff give extra time to gather the medicine, prepare room in the emergence ward or in the ICU and consult a physician.  
This ML model will help in prediction of early diagnosis of the disease and consequently help saving precious lives of the patients.


##### Dataset Link : https://www.kaggle.com/datasets/drscarlat/mimic2-original-icu/metadata
##### (Due to unknown reason the dataset has been removed from kaggle)
