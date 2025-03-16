Diabetes Prediction and Health Recommendations

Overview

This project is a machine learning-based system for predicting diabetes using the Pima Indians Diabetes dataset. The model is built using a Random Forest Classifier with hyperparameter tuning via GridSearchCV. Additionally, it provides personalized health recommendations based on patient input data.

Features

Data preprocessing (handling missing values, scaling features)

Hyperparameter tuning for Random Forest Classifier

Model evaluation (accuracy, classification report, confusion matrix)

User input-based diabetes prediction

Personalized health recommendations

Installation

Prerequisites

Ensure you have Python installed along with the necessary libraries. You can install them using:

pip install pandas numpy scikit-learn

Dataset

The dataset should be a CSV file (diabetes.csv) containing the following columns:

Pregnancies

Glucose

BloodPressure

SkinThickness

Insulin

BMI

DiabetesPedigreeFunction

Age

Outcome (Target variable: 0 = Non-Diabetic, 1 = Diabetic)

How to Run

Place diabetes.csv in the same directory as the script.

Run the script using:

python diabetes_prediction.py

Enter the required patient details when prompted.

The script will output the diabetes prediction along with personalized health recommendations.

Model Training

The dataset is split into training (80%) and testing (20%).

Standardization is applied using StandardScaler().

Hyperparameter tuning is performed using GridSearchCV.

The best Random Forest model is selected based on accuracy.

Example Output:

Best Parameters: {'max_depth': 15, 'min_samples_leaf': 1, 'min_samples_split': 5, 'n_estimators': 200}
Accuracy: 0.77

Diabetes Prediction (1=Diabetic, 0=Non-Diabetic): 0


Health Recommendations:
- Consider weight management programs.
- Monitor blood pressure and reduce salt intake.
- Consult a healthcare provider about insulin levels.


Customization

You can modify the health recommendations by adjusting the health_recommendations() function based on specific medical guidelines.

License

This project is open-source and free to use for educational purposes.


