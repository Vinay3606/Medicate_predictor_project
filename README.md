🧪 Project Overview
This project predicts the appropriate drug for patients based on their medical profile using machine learning. It includes:

Comprehensive data preprocessing and visualization

Feature engineering for improved predictions

Model training with Decision Tree and Random Forest

Hyperparameter tuning and model evaluation

Deployment-ready prediction function

📂 Dataset
drug200.csv - Contains patient information with the following features:

Age: Patient's age

Sex: Gender (M/F)

BP: Blood pressure level (HIGH, NORMAL, LOW)

Cholesterol: Cholesterol level (HIGH, NORMAL)

Na_to_K: Sodium-to-Potassium ratio

Drug: Target variable (5 drug types: DrugA, DrugB, etc.)
Data Loading & Exploration:

Loaded the drug200 dataset and examined its structure, missing values, and feature distributions.

📈Data Visualization:

Visualized class balance, feature distributions, pairwise relationships, correlations, and categorical feature breakdowns using countplots, boxplots, violin plots, pairplots, heatmaps, and stacked bar charts.

🧾Data Preprocessing:

Converted categorical features (Sex, BP, Cholesterol) to numeric using label encoding.

Engineered an AgeGroup feature for better pattern extraction.

💭Feature Selection:

Selected relevant features (Age, Sex, BP, Cholesterol, Na_to_K, AgeGroup) for modeling.

📝Train-Test Split:

Split the data into training and testing sets with stratification to preserve class distribution.

💉Model Training:

Trained Decision Tree and Random Forest classifiers for drug prediction.

🏅Model Evaluation:

Assessed models using accuracy, classification report, confusion matrix, feature importance, and visualized the decision tree.

Used t-SNE and ROC curves for advanced evaluation and error analysis.

✏️Hyperparameter Tuning:

Used GridSearchCV to optimize Random Forest parameters via cross-validation.

🏁Model Saving & Deployment:

Saved the best model and encoders for future predictions.

Provided a prediction function for new patient data.




📊 Key Visualizations
Drug Class Distribution - Shows balance of target variable

Age vs Drug Boxplot - Reveals age patterns for different drugs

Correlation Heatmap - Identifies feature relationships

Feature Importance - Highlights most predictive features

Confusion Matrix - Evaluates model performance per class

🧠 Algorithm Selection Rationale
Decision Tree: Simple, interpretable, provides clear decision rules

Random Forest: Handles overfitting, improves accuracy via ensemble learning

Why not others?:

Logistic Regression: Limited to linear relationships

SVM: Computationally expensive for multiclass

KNN: Sensitive to feature scaling

XGBoost: More complex but similar performance to RF here

💡 Future Improvements
Add more medical features (allergies, weight, genetic markers)

Implement neural networks for complex pattern detection

Build web interface for clinical use

Add dosage recommendation system

📝 Conclusion
This end-to-end project demonstrates a robust pipeline for drug classification that:

Handles real-world medical data preprocessing

Creates insightful visualizations

Implements interpretable ML models

Provides deployment-ready functionality

The Random Forest model achieved 98% accuracy with tuned hyperparameters, making it suitable for clinical decision support systems
