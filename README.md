# Credit-Risk-Model

## 💳 Credit Risk Prediction Web App
This project is a Credit Risk Classification Web App built with a machine learning model that predicts whether a loan application is likely to be Approved or Rejected based on user inputs. The model is deployed using Flask and hosted live on Render.

## 📊 Project Summary
Goal: Predict loan approval status using applicant details.

Model: Gradient Boosting Classifier (accuracy > 80% on train/test sets).

Frontend: HTML + CSS

Backend: Python (Flask)

Deployment: Render

## 🧪 Model Development Process
This project follows a full machine learning pipeline, from raw data to deployment:

### 1. Data Cleaning & Wrangling
Removed outliers using by inspecting the boxplot distributions.

Handled missing values and corrected inconsistent data entries.

### 2. Feature Engineering
Applied SimpleImputer to fill in missing values.

Scaled numerical features using StandardScaler for better model convergence.

Encoded categorical variables using OrdinalEncoder to retain ordinal relationships.

### 3. Handling Imbalanced Data
Used SMOTE (Synthetic Minority Oversampling Technique) to balance the dataset, which significantly improved the model's ability to correctly classify the minority class (Rejected loans).

### 4. Model Training
Built a streamlined pipeline using Pipeline() from sklearn to ensure clean, reproducible model training.

Evaluated multiple classifiers and selected Gradient Boosting Classifier due to its superior performance (Train/Test Accuracy > 80%).

### 5. Model Serialization
The trained pipeline was saved using pickle for fast loading and use in the Flask backend.



## 🗒️ Notes to reader
If you want to test out the model on Jupyter notebooks you can find the ipynb file in Credit-Risk-Model/Jupyter Notebook directory, additionally you will also find the dataset.
Now if you want to deploy this on your local machine please consider:
1. Downloading this project on your machine.
2. Install the libraries in the requirements.txt file
3. Change line 7 of app.py from "r'model.pkl'" to where you have put this pickle file in your machine.

## 🙋🏽 About the Author
Thomas Karabo — Aspiring AI Engineer passionate about solving real-world problems using Data Science and Machine Learning.
