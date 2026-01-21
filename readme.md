# Power Load Type Prediction

## 🧠 Objective
Develop a multiclass machine learning model to predict the type of electrical load — “Light_Load”, “Medium_Load” or “Maximum_Load” — using historical power consumption data.

## 🚀 Approach
- Time-aware train–test split (last month reserved for testing)
- Median imputation for missing values
- Feature engineering (temporal & cyclical features)
- Model training & comparison:
  - Logistic Regression (baseline)
  - Random Forest (best performer)
  - Gradient Boosting

## 📊 Final Result
- Best Model: **Random Forest (tuned)**
- Accuracy: ~92%
- F1 Score (weighted): ~92–93%

### Why This Model Works
Random Forest captures non-linear interactions and is robust to correlated features, making it ideal for electrical load prediction.

## 📁 Project Structure

```text
power-load-type-prediction/
├── data/
│   └── load_data.csv
├── notebooks/
│   └── Load_Type_Prediction.ipynb
├── README.md
└── requirements.txt

``` 
## How to Run
1. Clone the repository
2. Install dependencies using `pip install -r requirements.txt`
3. Run the Jupyter notebook in `notebooks/`

## Added Comments to highlight steps

## 📈 Notes
- Uses relative paths for portability
- Time-aware split prevents data leakage
- Avoids dropping rows with missing values
