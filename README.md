🎓 Predicting Student Depression: A Machine Learning & Explainable AI Approach
This project develops a data-driven, interpretable machine learning framework to predict student depression using accessible academic and non-academic factors. The ultimate goal is to create a transparent and reliable tool that educational institutions can use to proactively support student mental health.

🚀 Project Goal
The primary objective is to build a highly accurate classification model to identify students at risk of depression, using non-clinical data. By integrating Explainable AI (XAI), the project aims to:

Provide actionable insights into the key drivers of mental distress.

Enable trustworthy decision-support for early intervention.

📊 Key Findings & Results
After evaluating 10 machine learning models, the SMOTE-enhanced XGBoost model emerged as the top performer.

Top Model: Tuned XGBoost + SMOTE

Test ROC-AUC Score: 0.94

Key Predictors (via SHAP interpretation):

History of suicidal thoughts

High academic pressure

Financial stress

⚙️ Machine Learning Pipeline
Data Preprocessing

Handled missing values

Applied feature encoding

Reduced features using correlation analysis

Handling Class Imbalance

Applied SMOTE (Synthetic Minority Over-sampling Technique) to prevent bias and improve model robustness

Model Training & Evaluation

Trained 10 supervised learning models

Evaluated with multiple metrics (focus on ROC-AUC)

Model Interpretation

Used SHAP (SHapley Additive exPlanations) for transparency and explainability

📈 Model Performance Summary
Model	Accuracy	F1-Score	ROC-AUC
SMOTE + XGBoost (Tuned)	86.7%	86.7%	0.941
Advanced Stacking	86.6%	86.6%	0.939
Stacking Ensemble	84.6%	84.5%	0.919

🛠️ How to Use
Clone the repository:

bash
Copy
Edit
git clone [your-repo-link]
cd [your-repo-folder]
Install dependencies:

bash
Copy
Edit
pip install pandas numpy scikit-learn xgboost shap matplotlib seaborn jupyter
Run the Jupyter Notebook:

bash
Copy
Edit
jupyter notebook full.ipynb
💡 Challenges & Future Improvements
Challenges

The dataset was highly imbalanced → resolved using SMOTE.

Future Work

Longitudinal Data: Incorporate multiple academic terms for tracking mental health trends.

Real-Time Deployment: Build an ethical dashboard for counselors or a confidential self-assessment tool for students.

Fairness Audits: Ensure equitable model performance across demographic groups.
