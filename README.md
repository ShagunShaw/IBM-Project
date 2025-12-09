# Heart Disease Prediction using Logistic Regression

## 📋 Project Overview
This is an IBM project focused on predicting the risk of heart disease using Logistic Regression. The project uses the Framingham Heart Study dataset to analyze various health indicators and predict the 10-year risk of coronary heart disease (CHD).

## 🔗 Google Colab Link
Access the project notebook here: [Google Colab](https://colab.research.google.com/drive/1nKBoNYX2oRp-mi76fq9DSKrGkT_W-oAa?usp=drive_link)

## 📊 Dataset
The project uses the **Framingham Heart Study dataset** (`framingham.csv`), which contains various health metrics and demographic information to predict heart disease risk.

## 🛠️ Technologies Used
- **Python** - Programming language
- **NumPy** - Numerical computing
- **Pandas** - Data manipulation and analysis
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Scikit-learn** - Machine learning library

## 🔍 Project Workflow

### 1. Data Preprocessing
- **Data Loading**: Imported the Framingham dataset
- **Data Exploration**: Analyzed dataset shape, structure, and statistics
- **Feature Engineering**: Removed the `education` column
- **Data Type Conversion**: Converted `cigsPerDay` and `BPMeds` to Int64

### 2. Handling Missing Values
- Filled missing values in `cigsPerDay` and `BPMeds` with 0
- Imputed missing values in `glucose` and `totChol` using quantile method
- Removed remaining rows with missing values

### 3. Outlier Detection & Removal
- **Glucose**: 
  - Visualized distribution using histograms
  - Removed outliers using 5th and 95th percentile bounds
- **Total Cholesterol**: 
  - Plotted distribution to identify outliers
  - Filtered data based on 5th and 95th percentile thresholds

### 4. Model Training
- Split data into features (X) and target variable (y)
- Target variable: `TenYearCHD` (10-year risk of coronary heart disease)
- Used 70-30 train-test split with stratification
- Trained a **Logistic Regression** model

### 5. Model Evaluation
- **Accuracy Score**: Evaluated model performance on test data
- **Classification Report**: Generated precision, recall, and F1-score metrics
- **Confusion Matrix**: Visualized prediction results using a heatmap

## 📈 Key Features
✅ Comprehensive data cleaning and preprocessing  
✅ Statistical handling of missing values  
✅ Outlier detection and removal techniques  
✅ Visual data analysis with plots and histograms  
✅ Machine learning model implementation  
✅ Performance evaluation with multiple metrics  

## 📁 Project Structure
```
.
├── framingham.csv          # Dataset file
├── IBM_Project.ipynb       # Jupyter notebook with complete analysis
└── README.md              # Project documentation
```

## 🚀 Getting Started

### Prerequisites
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Running the Project
1. Clone this repository
2. Ensure `framingham.csv` is in the project directory
3. Open and run `IBM_Project.ipynb` in Jupyter Notebook or Google Colab

## 📊 Model Performance
The model's performance is evaluated using:
- Accuracy percentage
- Precision, Recall, and F1-Score
- Confusion Matrix visualization

## 👤 Author
**Shagun Shaw**

## 📝 License
This project is part of an IBM learning initiative.

---
*This project demonstrates end-to-end machine learning workflow from data preprocessing to model evaluation for heart disease prediction.*
