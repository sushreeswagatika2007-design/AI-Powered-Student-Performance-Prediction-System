Run Command: python student_performance_system.py
​Dataset: data/student_performance_data.csv (600 cleaned student rows, 10 features, 3 target tiers).
​Workflow:
​1. Clean data (drop duplicates + median/mode imputation).
​2. Preprocess (StandardScaler + OneHotEncoder inside a ColumnTransformer).
​3. Train & compare 3 models via 5-Fold Stratified Cross-Validation.
​4. Save winning pipeline (models/best_student_performance_model.joblib).
​5. Run interactive terminal CLI to predict performance & give study advice.
​Key Results:
​Logistic Regression (Winner): 95.00% Accuracy (0.9415 CV F1)
​Random Forest: 91.67% Accuracy
​Decision Tree: 86.67% Accuracy
