# This project aims to build a machine learning model that can predict the likelihood of a person having a stroke based on various demographic, lifestyle, and health factors.

Dataset

The dataset used in this project is the Stroke Prediction Dataset from Kaggle. It contains information on 5110 patients, including demographic data (age, gender), lifestyle factors (smoking status, work type, residence type), health data (hypertension, heart disease, BMI), and the target variable (stroke or no stroke).

Requirements

The following packages are required to run this project:

. pandas
. numpy
. scikit-learn
. seaborn
. matplotlib


You can install these packages using pip by running the following command:


#pip install pandas numpy scikit-learn seaborn matplotlib


Usage

To run this project, run the stroke_predictor.py file. This file contains the code to preprocess the data, train the machine learning model, and evaluate its performance. The final model is saved to a file named stroke_prediction_model.pkl.

Results

After training and evaluating several machine learning models, the best-performing model was found to be a Random Forest Classifier with an accuracy of 0.95 and an F1 score of 0.38. This model can be used to predict the likelihood of a person having a stroke based on their demographic, lifestyle, and health factors.

Conclusion

This project demonstrates the potential of machine learning in predicting the likelihood of a person having a stroke. However, it should be noted that the accuracy of the model is not perfect, and further research is needed to improve its performance. Nevertheless, this model can be used as a tool to identify individuals who may be at a higher risk of having a stroke and take necessary preventive measures.




