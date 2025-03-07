# DiabetesMind: AI-Powered Diabetes Prediction

DiabetesMind is a machine learning project designed to predict diabetes risk using patient health metrics. It focuses on exploratory data analysis (EDA), feature engineering, and model optimization to improve accuracy despite a small dataset (768 samples).

## Key Features
- Handles missing values and outliers using Winsorization and log transformation.
- Creates new predictive features (Glucose_BMI Interaction, Pregnancy-Age Ratio, BMI Encoding).
- Balances dataset using Random Over-Sampling (ROS) and scales features with StandardScaler.
- Trains and optimizes Logistic Regression, SVM, Random Forest, and Gradient Boosting.
- Evaluates models using F1-score, precision, recall, and confusion matrices.

## Technologies Used
- **Machine Learning:** Logistic Regression, SVM, Random Forest, Gradient Boosting  
- **Data Processing:** Pandas, NumPy, Winsorization, Feature Engineering   
- **Model Optimization:** GridSearchCV, RandomizedSearchCV, Hyperparameter Tuning  
- **Data Balancing:** Random Over-Sampling (ROS)  
- **Visualization:** Matplotlib, Seaborn, Heatmaps, Boxplots  

