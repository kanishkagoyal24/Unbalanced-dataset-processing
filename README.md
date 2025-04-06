# Unbalanced-dataset-processing
Imbalanced Dataset Handling with Resampling Techniques (Diabetes Prediction)
This project demonstrates how to handle imbalanced classification datasets using various resampling techniques and class weighting strategies. The dataset used is the Pima Indians Diabetes Dataset, a popular dataset in the machine learning community, available via the UCI repository.

📁 Dataset
The dataset is loaded from UCI ML Repository.
It consists of 768 samples with 8 medical features such as glucose level, BMI, age, etc., and a binary outcome variable (Outcome) indicating whether a patient has diabetes (1) or not (0).

🧪 Project Flow
1. Basic Exploration & Visualization
Dataset structure and statistical summary

Class distribution analysis

Feature correlation heatmap

Pie chart for visualizing class imbalance

2. Preprocessing
Feature scaling using StandardScaler

Train-test split with stratification

3. Model Training
Base model: RandomForestClassifier

Model evaluation metrics: Accuracy, F1 Score, and AUC (ROC Area Under Curve)

⚖️ Resampling Techniques Used
Technique	Description
1) Original -	No balancing done
2) Random Oversampling - Duplicate samples from the minority class to balance the dataset
3) Random Undersampling	- Remove samples from the majority class to match the minority class
4) SMOTE	Synthetic Minority Over-sampling Technique — creates synthetic samples
5) Tomek Links -	Removes ambiguous overlapping samples between classes
6) Class Weights -	Penalizes the model more for misclassifying the minority class

✅ Best AUC was achieved using Tomek Links, indicating better distinction between classes
🔥 Best F1 Score was achieved using Random Undersampling, suggesting better balance between precision and recall

🛠 Tools & Libraries
Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

imblearn (SMOTE, Tomek Links, etc.)

📂 How to Run
Open this notebook in Google Colab or Jupyter.

Run the cells step-by-step to view results.

Install dependencies if needed:

bash
Copy
Edit
pip install imbalanced-learn
📌 Use Case
This notebook can be used as a template or learning guide for:

Handling imbalanced datasets

Comparing multiple sampling techniques

Evaluating models using F1 and AUC metrics

