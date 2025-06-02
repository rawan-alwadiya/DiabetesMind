# DiabetesMind: Predictive Modeling for Diabetes Diagnosis

DiabetesMind is an AI-powered system designed to predict diabetes diagnoses using medical and patient profile data. The project leverages advanced preprocessing, robust feature engineering, and ensemble-based machine learning models to deliver accurate predictions on a small, imbalanced clinical dataset.

---

## Dataset

- **Dataset**: [Pima Indians Diabetes Database](https://www.kaggle.com/datasets/jhskaggle/diabetescsv)
- **Samples**: 768
- **Features**: 8 medical/patient attributes + 1 target (Outcome)

---

## Key Features

### Binary Classification Model
- Predicts whether a patient is diabetic or not based on health indicators.
- Achieved **F1 Score** of **87.2%** and **Recall** of **92.9%**.
- Demonstrates strong sensitivity to diabetic cases.

### Preprocessing & Feature Engineering
- **Missing Value Treatment**:
  - Treated medically implausible values (e.g., 0 Glucose or BMI) as missing.
  - Dropped rows with 3+ missing critical values to retain data quality.
  - Used models like **XGBoost** and **LightGBM** that natively handle missing data.

- **Outlier Analysis**:
  - Detected using domain-specific thresholds and visualizations.
  - Removed implausible values and retained medically valid extremes.
  - Applied **standardization** to reduce the influence of extreme values.

- **Class Imbalance Handling**:
  - Applied **oversampling** on minority class (diabetic patients).
  - Enhanced model's ability to generalize without introducing synthetic noise.

- **Feature Construction**:
  - Developed new features by combining existing attributes through **ratios and interactions** (e.g., Glucose_BMI) to capture complex patterns.
  - These engineered features helped improve model performance by extracting richer information from the dataset.

- **Skewness Correction & Scaling**:
  - Applied **Yeo-Johnson transformation** to reduce skewness and normalize non-Gaussian distributions.
  - Performed **standard scaling** to normalize feature magnitudes and minimize the impact of extreme values across all numerical features.

---

## Model Performance

- **Best Model**: Random Forest
  - **F1 Score**: **87.2%**
  - **Recall**: **92.9%**
  - Strong recall ensured effective detection of diabetic patients.
- **Other Competitive Models**:
  - **XGBoost, LightGBM, CatBoost, and HistGradientBoosting**
  - All benefited from engineered features and data preprocessing strategies.

---

## Technology Stack

- **Machine Learning Models**: Random Forest, XGBoost, LightGBM, CatBoost, HistGradientBoosting
- **Preprocessing & Feature Engineering**: Pandas, NumPy, SciKit-Learn
- **Outlier & Missing Value Handling**: Domain-based thresholding, NaN strategies
- **Evaluation Metrics**: F1 Score, Recall, Accuracy, Precision, Confusion Matrix
- **Visualization**: Matplotlib, Seaborn

---

## Project Highlights

- Achieved **87.2% F1 Score** with **92.9% recall**, ensuring accurate identification of diabetic patients.
- Implemented a thorough **data cleansing and transformation pipeline** suited for clinical data.
- Designed a **robust feature engineering strategy** that extracted meaningful insights from limited data.
- Leveraged **ensemble models** to achieve optimal performance despite a small, imbalanced dataset.

---
