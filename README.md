Overview of Project: Pima Indian Diabetes Prediction

Project Title

Pima Indian Diabetes Prediction using Support Vector Machine (SVM)

Overview of the Project

This project implements an end-to-end machine learning pipeline that classifies patients as either diabetic or non-diabetic based on diagnostic health data. Using the Pima Indian Diabetes Dataset, the main objective is to develop a reliable classification model that may be helpful in early risk assessment. It involves rigorous data standardization, splitting the data into training and test sets, and the actual training of a Support Vector Classifier. The final result is a high-accuracy model with strong generalization capability-that is, low overfitting-on unseen patient data.

Features

The model makes a prediction based on eight quantitative diagnostic features:

Pregnancies: Number of times pregnant.

GLUCOSE: Plasma glucose concentration a 2 hours in an oral glucose tolerance test.

BloodPressure: Diastolic blood pressure (mm Hg).

SkinThickness: Triceps skin fold thickness (mm).

Insulin: 2-Hour serum insulin (mu U/ml).

BMI: Body mass index (weight in kg/(height in m)^2).

DiabetesPedigreeFunction: A function that determines risk based on family history.

Age: Age in years.

The Target Feature is Outcome: 0 - Non-Diabetic, 1 - Diabetic

● Technologies/Tools Used

Category

Technology/Tool

Role in Project

Programming Language

Python 3.x

Core implementation language.

Development Environment

Jupyter Notebook

Used for interactive coding, analysis, and documentation.

Data Manipulation

Pandas

Used for loading the dataset and general handling of data.

Numerical Computing

NumPy

Used for efficient array operations, especially reshaping of data.

Machine Learning

Scikit-learn (sklearn)

Import the essential ML components: StandardScaler, train_test_split, svm.SVC and accuracy_score.

● Steps to Install & Run the Project

This project is run within a standard Python environment, typically a Jupyter Notebook or a Python IDE.

Prerequisites (Dependencies)

You need to have Python 3 installed. Install the libraries you need with pip:

pip install numpy pandas scikit-learn


Running the Notebook

Obtain Data: Make sure that the data file, diabetes dataset.csv, is in the same folder as your project notebook.

Open Notebook: Open your Jupyter Notebook environment and open the Diabetes Prediction.ipynb file.

Execute Cells: Run the cells in order from top to bottom.

The first few cells handle imports and loading of data.

Data standardization and the train/test split are performed in subsequent cells.

The model training and evaluation cells will output the Training and Test Accuracies.

The last cell shows a single-point prediction.

Following are test instructions:

The Hold-out Method is used for testing the project, which involves an 80/20 split.

1. Testing of Generalization

Check Accuracy Scores: Using the outputs provided by executing the model training and evaluation cells, compare the Training Data Accuracy vs. the Test Data Accuracy.

Goal: The test accuracy, approximately 77.27%, should be very close to the training accuracy, approximately 78.66%.

Pass Condition: A small difference, less than 2%, implies that the model has generalized well and is ready for use.

2. Live Prediction Test

Modify Input Data: In the last code cell, replace the sample input data with a new set of 8 standardized health measures for a hypothetical patient.

The format must be a tuple of 8 numbers, e.g., (1, 85, 66, 29, 0, 26.6, 0.351, 31) Run Prediction: The following cell execution shows the system classifying the new input for either "Person is Diabetic" or "Person is not Diabetic."
