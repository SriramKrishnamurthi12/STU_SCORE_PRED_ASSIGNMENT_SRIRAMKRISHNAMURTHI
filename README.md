Student Score Prediction using Linear Regression

Problem Statement
The objective of this project is to predict a student’s final exam score based on academic and lifestyle-related factors. The goal is to understand how different variables such as study hours and attendance influence academic performance using a machine learning model.

Dataset Description
A custom dataset was created using Pandas. The dataset contains 15 records and includes the following features:
Study_Hours – Number of hours the student studies per day
Attendance – Attendance percentage
Sleep_Hours – Average sleep per day
Practice_Test_Score – Score obtained in practice tests
Exam_Score – Final exam score (target variable)
The dataset was manually created for learning and experimentation purposes.

Data Exploration
Basic exploratory analysis was performed, including:
Viewing first and last five rows
Checking dataset shape
Inspecting data types
Checking for missing values
The dataset did not contain any missing values and was clean for training.

Data Visualization
The following visualizations were created:
Scatter plot to analyze relationship between Study Hours and Exam Score
Histogram to observe distribution of Exam Scores
Boxplot to understand spread of Attendance
These visualizations helped identify positive relationships between study-related features and exam performance.

Model Used
Linear Regression from scikit-learn was used to train the model.
Steps followed:
Split dataset into training and testing sets
Trained the Linear Regression model
Evaluated performance using Mean Absolute Error (MAE) and R2 Score

Results
The model achieved a good R2 score, indicating that the independent variables explain a significant portion of the variation in exam scores.
The MAE value was relatively low, meaning the predicted scores were close to actual scores.
When removing one feature (Sleep_Hours), the performance slightly changed, indicating it had limited influence.
When adding Practice_Test_Score, the performance improved, showing that practice test performance is an important predictor of final exam score.

Overfitting Check
The model was also trained on the full dataset without splitting. The R2 score was higher in this case, but this does not reflect real-world performance.
Overfitting occurs when a model learns the training data too well, including noise, and performs poorly on unseen data. Proper train-test splitting is necessary to evaluate generalization.

Conclusion
This project demonstrates how Linear Regression can be used to predict academic performance based on relevant features. Study hours, attendance, and practice test scores showed strong influence on final exam results.

The experiment also highlighted the importance of feature selection and proper model evaluation techniques to avoid overfitting.
