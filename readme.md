# Power System Load Type Prediction

## Objective
Predict the load type of a power system (Light, Medium, Maximum) using historical power consumption data.

## Approach
- Time-aware train-test split (last month as test set)
- Median imputation for missing numerical values
- Feature engineering using time-based and cyclical features
- Model comparison: Logistic Regression, Random Forest, Gradient Boosting
- Hyperparameter tuning using GridSearchCV

## Final Model
Random Forest Classifier (Tuned)

## Results
- Accuracy: ~92%
- F1-score (weighted): ~0.93

## How to Run
1. Clone the repository
2. Install dependencies using `pip install -r requirements.txt`
3. Run the Jupyter notebook in `notebooks/`

## Added Comments to highlight steps