# COVID-19 Patient Symptoms & Diagnosis Analysis

## 📊 Project Overview

This data analysis project explores COVID-19 patient symptoms, demographics, and diagnosis outcomes using machine learning classification models. The analysis examines the relationship between various symptoms, comorbidities, patient demographics, and COVID-19 test results.

## 🎯 Objectives

- Analyze the distribution of COVID-19 symptoms across different patient demographics
- Identify correlations between symptoms, comorbidities, and COVID-19 positive results
- Build and compare multiple machine learning models for COVID-19 diagnosis prediction
- Visualize patterns in patient data to gain insights into disease indicators

## 📁 Dataset

**File:** `covid19_patient_symptoms_diagnosis.csv`

**Features (17 columns):**

- **Patient Information:** patient_id, age, gender
- **Symptoms (Binary):** fever, dry_cough, sore_throat, fatigue, headache, shortness_of_breath, loss_of_smell, loss_of_taste, chest_pain
- **Health Metrics:** oxygen_level, body_temperature
- **Medical History:** comorbidity (Diabetes, Asthma, Heart Disease, None)
- **Exposure:** travel_history, contact_with_patient
- **Target Variable:** covid_result (0 = Negative, 1 = Positive)

**Dataset Size:** 5,001 patient records

## 🔍 Analysis Performed

### 1. Exploratory Data Analysis (EDA)

- Data cleaning and handling missing values in comorbidity field
- Distribution analysis of comorbidities
- Gender-based symptom analysis (dry cough, headache)
- Travel history correlation with COVID-19 results
- Visual exploration using bar plots and count plots

### 2. Data Preprocessing

- Label encoding for categorical variables (gender, comorbidity)
- Train-test split (70% training, 30% testing)
- Feature-target separation

### 3. Machine Learning Models

Four classification algorithms were implemented and evaluated:

| Model                               | Accuracy Score |
| ----------------------------------- | -------------- |
| **Logistic Regression**             | ~0.74          |
| **Decision Tree Classifier**        | ~0.95          |
| **Random Forest Classifier**        | ~0.97          |
| **Support Vector Classifier (SVC)** | ~0.74          |

**Best Performing Model:** Random Forest Classifier (97% accuracy)

### 4. Correlation Analysis

- Examined feature correlations to identify key predictors
- Analyzed relationships between symptoms and diagnosis outcomes

## 🛠️ Technologies Used

- **Python 3.x**
- **Libraries:**
  - `pandas` - Data manipulation and analysis
  - `numpy` - Numerical computing
  - `matplotlib` - Data visualization
  - `seaborn` - Statistical data visualization
  - `scikit-learn` - Machine learning algorithms
    - LogisticRegression
    - DecisionTreeClassifier
    - RandomForestClassifier
    - SVC (Support Vector Classifier)
    - LabelEncoder
    - train_test_split

## 📈 Key Insights

1. **Random Forest** and **Decision Tree** models significantly outperform linear models for COVID-19 diagnosis prediction
2. Multiple symptoms and patient characteristics are strong indicators when combined
3. Comorbidity distribution shows variation across gender groups
4. Travel history shows correlation with COVID-19 positive results

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Running the Analysis

1. Clone this repository
2. Ensure the dataset is in the `datasets/` folder
3. Open `COVID-19 Patient Symptoms & Diagnosis.ipynb` in Jupyter Notebook or VS Code
4. Run all cells sequentially

## 📊 Visualizations

The notebook includes various visualizations:

- Bar plots for comorbidity distribution
- Count plots for symptom analysis by gender
- Travel history vs COVID-19 result analysis
- Correlation heatmap (available in the notebook)

## 📝 Future Improvements

- Feature importance analysis to identify top predictors
- Hyperparameter tuning for model optimization
- Cross-validation for more robust performance metrics
- ROC curves and confusion matrices for detailed model evaluation
- Analysis of false positives and false negatives
- Time-series analysis if temporal data is available

## 👤 Author

Data Analysis Project - COVID-19 Patient Symptoms & Diagnosis

## 📄 License

This project is for educational and analytical purposes.

---

**Note:** This analysis is for educational purposes only and should not be used as a substitute for professional medical diagnosis.
