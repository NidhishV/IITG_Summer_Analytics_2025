# Nutrition Health Survey- Age Prediction

This project involves building a classification model to predict whether an individual is a Senior (65+) or an Adult (under 65) based on a subset of health, lifestyle, and lab test features from the NHANES dataset (National Health and Nutrition Examination Survey), provided for the Summer Analytics 2025 Hackathon in collaboration with the Consulting and Analytics Club, IIT Guwahati.

⸻

Objective

To develop a machine learning model that predicts the target variable age_group:
	•	Adult → 0
	•	Senior → 1

Predictions were evaluated using the F1 Score to ensure balanced performance across both classes.

⸻

Data Preprocessing
	•	Dropped Identifier: SEQN (not predictive)
	•	Handled Missing Values:
	•	Categorical columns (RIAGENDR, DIQ010, PAQ605) filled with mode
	•	Numerical columns filled with mean
	•	Special codes (7, 9) in PAQ605 were treated as missing
	•	Label Encoding:
	•	Converted age_group from string labels ("Adult", "Senior") to integers (0, 1)
	•	Feature Scaling: Standardized all features using StandardScaler

⸻

Model Training
	•	Used a Random Forest Classifier with:
	•	n_estimators = 200
	•	random_state = 42
	•	Performed an 80/20 stratified train-validation split to preserve class distribution

⸻

Evaluation
	•	The model achieved an F1 Score of 1.0 on the validation set
	•	Indicates perfect classification performance on the given data (no misclassifications)

⸻

Submission
	•	Final predictions on the test set were saved in a CSV file with a single column: age_group
	•	Format matched the provided sample_submission.csv
	•	Submission file contains 312 rows with values 0 or 1

⸻

Tools & Libraries
	•	Python (Pandas, NumPy, scikit-learn)
	•	Jupyter Notebook for experimentation and visualization

⸻

Files Included
	•	Train_Data.csv: Training dataset with features + target
	•	Test_Data.csv: Test dataset with features only
	•	submission.csv: Final predictions for test data
	•	notebook.ipynb: Code for preprocessing, training, evaluation, and submission
