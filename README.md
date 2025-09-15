**💼 Predicting Employee Promotions Using HR Analytics**

**Why This Project?**

Understanding which employees are likely to be promoted helps HR teams make fair, data-backed decisions. In this project, I built and compared three machine learning models—Logistic Regression, Decision Tree, and KNN—to predict promotion eligibility using employee performance, training, education, and other HR factors.

**What you will find in this project?
**
EDA- Department-level promotion trends, education impact, KPI completion analysis
Data Prep- Missing values handled, one-hot encoded categoricals, scaled numerics
Modeling- Logistic Regression, Decision Tree, KNN pipelines with GridSearchCV tuning
Evaluation- Accuracy, precision, recall, F1 scores across models
Final Pick- KNN performed best overall, Decision Tree helped explain feature impact


**My Approach**

1. Data Cleaning & Transformation
	•	Dropped duplicates and handled missing values (e.g., filled education with mode).
	•	One-hot encoded department, education, gender, etc.
	•	Scaled numeric features with StandardScaler.

2. Exploratory Data Analysis
	•	Promotion counts by department, education, and KPI score
	•	Boxplots for previous year rating vs promotion
	•	Uncovered trends like high KPI scores strongly correlating with promotions

3. Feature Engineering
	•	Selected and scaled key numerical features
	•	Kept only relevant one-hot encoded fields
	•	Prepared dataset for classification models

4. Modeling
	•	Built pipelines using Pipeline and ColumnTransformer
	•	Trained three models: Logistic Regression, Decision Tree, KNN
	•	Performed hyperparameter tuning using GridSearchCV

5. Evaluation & Diagnostics
	•	Evaluated all models using accuracy, precision, recall, and F1 score
	•	KNN achieved 89% accuracy and 88% F1 score, outperforming others
	•	Decision Tree helped identify which features (like training score, rating) mattered most

6. Prediction Logic
	•	Final KNN model can predict promotions based on training score, performance, education, and other encoded attributes

**Business Impact**

HR teams often struggle to balance fairness, performance, and policy when deciding promotions. This model helps take the guesswork out. With accurate predictions based on training scores, performance ratings, and other employee factors, the system can:
	•	Improve transparency in promotion decisions by relying on data-backed patterns instead of gut instinct
	•	Support diversity and inclusion by highlighting underrepresented candidates who meet the same performance criteria
	•	Save time by narrowing the focus to strong contenders, reducing hours spent reviewing profiles manually
	•	Prevent attrition by identifying high performers who may leave if passed over unfairly
	•	Guide upskilling and training programs by showing which factors (like KPI completion or prior training) matter most for career growth

What this really means is: instead of waiting for performance reviews to figure out who’s ready for the next step, HR can proactively identify and support talent with data.
