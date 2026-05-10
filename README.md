# A-Comparative-Study-of-an-Individual-Ensemble-ML-Models-for-Brain-Stroke-Risk-Prediction

📌 Project Overview:
This project presents a comparative study of individual and ensemble machine learning models to predict the risk of brain stroke in patients. Using clinical and lifestyle-based features, the models classify patients as at-risk or not at-risk of experiencing a stroke.
The study evaluates four ML classifiers — Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting — alongside a Soft Voting Ensemble that combines all four models to achieve superior predictive performance.

🎯 Objective:
Compare individual ML models vs. ensemble techniques for stroke risk prediction.
Identify the most accurate and reliable model using standard evaluation metrics.

🔬 Methodology:
Exploratory Data Analysis (EDA) — Distribution plots, correlation heatmap, class balance check.
Data Preprocessing — Missing value imputation, StandardScaler for numerical features, OneHotEncoding for categorical features.
Leakage Removal — Dropped near-diagnostic leakage features (anxiety_doom, irregular_heartbeat, excessive_sweating) and the derived stroke_risk_percentage column.
Train-Test Split — 80/20 stratified split with random_state=42.
Model Training — Pipelines built for each model (preprocessor + classifier).
5-Fold Cross-Validation — Evaluated using ROC AUC score.
Ensemble (Voting Classifier) — Soft voting combining all four model pipelines.
Evaluation — Accuracy, Precision, Recall, F1 Score, ROC AUC, and Confusion Matrix.

📋 Prediction UI:
The project includes an ipywidgets-based interactive interface where users can input patient symptoms and receive:
🔴 HIGH RISK / 🟢 NOT AT RISK classification
Stroke risk probability score
Stroke risk percentage

📰 Publication:
This research has been published in the International Journal of Engineering Development and Research (IJEDR).
📄 Paper: IJEDR26A1376_KiranSitap_Published_ResearchPaper.pdf
🏅 Certificate: IJEDR_Published_ResearchPaper_Certificate.jpg
