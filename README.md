Overview of Project: Pima Indian Diabetes Prediction

1) Project Title

Pima Indian Diabetes Prediction using Support Vector Machine (SVM)

2) Overview of the Project

This project involves creating a complete machine learning solution that categorizes patients as either diabetic or non-diabetic using diagnostic health data.
The Pima Indian Diabetes Dataset is used to build a model that can assist in early risk assessment. The project includes several key steps such as standardizing the data, dividing it into training and testing sets, and training a Support Vector Classifier. The final model is accurate and capable of performing well on new, unseen patient data with minimal overfitting.

3) Features

The model uses eight numerical diagnostic features to make its predictions:

Pregnancies: The number of times the patient has been pregnant.


GLUCOSE: The plasma glucose level measured two hours after an oral glucose tolerance test.


BloodPressure: The diastolic blood pressure in millimeters of mercury.


SkinThickness: The thickness of the triceps skin fold in millimeters.


Insulin: The serum insulin level measured two hours after an oral glucose tolerance test in micro U per milliliter.


BMI: The body mass index calculated by dividing the patient’s weight in kilograms by the square of their height in meters.


DiabetesPedigreeFunction: A value that estimates the risk based on family history of diabetes.


Age: The patient's age in years.


The target feature is the Outcome, which is either 0 for non-diabetic or 1 for diabetic.


4) Technologies/Tools Used

Category

Technology/Tool

Role in Project

Programming Language

Python 3.x

The primary language used for development.


Development Environment

Jupyter Notebook

Used for interactive coding, analysis, and documentation.


Data Manipulation

Pandas

Helps in loading and managing the dataset.


Numerical Computing

NumPy

Used for performing efficient array operations, especially for reshaping data.


Machine Learning

Scikit-learn (sklearn)

Provides essential machine learning components such as StandardScaler, train_test_split, svm.SVC, and accuracy_score.


5) Steps to Install & Run the Project

This project can be executed in a standard Python environment, such as Jupyter Notebook or a Python Integrated Development Environment (IDE).


Prerequisites (Dependencies)

Ensure that Python 3 is installed.
Install the required libraries using pip:

pip install numpy pandas scikit-learn

Running the Notebook

Obtain Data: Place the data file diabetes dataset.csv in the same directory as your project notebook.


Open Notebook: Launch your Jupyter Notebook and open the Diabetes Prediction.ipynb file.


Execute Cells: Run the cells in sequence from top to bottom.


The initial cells are used for importing libraries and loading the data.


Subsequent cells perform data standardization and split the data into training and testing sets.


The model training and evaluation cells provide the Training and Test Accuracies.


The final cell demonstrates a single-point prediction.


6) Test Instructions

The Hold-out Method is used for testing, which separates the data into an 80/20 split.


1.
Testing Generalization

Check Accuracy Scores: Compare the Training Data Accuracy and Test Data Accuracy using the outputs from the model training and evaluation cells.


Goal: The test accuracy, around 77.27%, should closely match the training accuracy, approximately 78.66%.


Pass Condition: A small difference, less than 2%, indicates that the model has generalized well and is ready for use.


2.
Live Prediction Test

Modify Input Data: In the last code cell, replace the sample input with a new set of 8 standardized health measures for a hypothetical patient.


The input should be in the format of a tuple of 8 numbers, for example, (1, 85, 66, 29, 0, 26.6, 0.351, 31).


Run Prediction: Execute the relevant cell to have the system classify the new input as either "Person is Diabetic" or "Person is not Diabetic."
