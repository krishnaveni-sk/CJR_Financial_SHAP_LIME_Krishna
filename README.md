 CJR Financial SHAP & LIME Project — Krishna

This project demonstrates interpretable machine learning using SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-Agnostic Explanations) for financial time-series prediction.
The project was completed as part of the Cultus Job Readiness (CJR) Program.

 Project Structure
├── CJR_Financial_SHAP_LIME_Krishna.ipynb   # Main notebook (full workflow)
├── processed_financial_dataset.csv         # Preprocessed dataset
├── X_test_data.csv                         # Test features
├── Y_test_data.csv                         # Test labels
├── shap_summary.png                        # SHAP global feature importance
├── shap_local_0.png to shap_local_9.png    # SHAP local explanations (10 instances)
├── lime_local_0.html to lime_local_9.html  # LIME local explanations (10 instances)
└── README.md                               # Project documentation

 Project Goal

To predict 5-day future stock movement and understand why the model makes each prediction using interpretability methods.

Two models were trained:

XGBoost Classifier

Neural Network Classifier

Both models were analyzed using:

✔ Global interpretability — Feature importance

✔ Local interpretability — Instance-wise explanations

✔ Comparative analysis — SHAP vs LIME

 Technologies Used

Python

Google Colab

Pandas, NumPy

scikit-learn

XGBoost

TensorFlow / Keras

SHAP

LIME

Matplotlib / Seaborn

 Steps Performed
1️⃣ Data Preparation

Loaded the financial dataset from CSV

Checked for stationarity

Created lag features

Created short-term return & volatility features

Split into train/test sets

2️⃣ Model Training

Two non-linear models were trained:

XGBoost Classifier

Neural Network Classifier (TensorFlow)

Hyperparameters were tuned using:

Learning rate adjustments

Depth changes

Optimizer tuning

Batch size variation

3️⃣ SHAP Analysis

Generated:

Global Summary Plot

Top feature contributions

Local explanations (10 instances) using waterfall plots

Files saved:

shap_summary.png
shap_local_0.png ... shap_local_9.png

4️⃣ LIME Analysis

For the same 10 instances:

Generated HTML explanation files

Highlighted positive & negative contributions

Compared LIME vs SHAP reasoning

Files saved:

lime_local_0.html ... lime_local_9.html

5️⃣ Comparative Interpretation

A complete text-based comparison was generated:

Stable patterns from SHAP

Instance-specific variations from LIME

Why certain features strongly influence volatility

Practical insights useful for financial analysts

 Key Insights

Lag-based features and volatility indicators were the strongest predictors.

SHAP showed consistent dominance of Lag1, Return_5d, Volatility_5d.

LIME provided deep clarity for each individual prediction.

Both models agreed on major drivers, increasing confidence in predictions.

 Deliverables Included

✔ Preprocessed dataset
✔ Model training code
✔ Hyperparameter tuning
✔ SHAP global & local explanations
✔ LIME explanations (10 instances)
✔ Comparative analysis
✔ Complete README documentation

 Author

Krishnaveni S
Cultus Job Readiness Program
Interpretable ML Project — SHAP & LIME
