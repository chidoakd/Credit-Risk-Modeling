# German Credit Risk Modeling

This project analyzes and models credit risk using the German Credit Data dataset. The workflow includes data loading, data transforming, data exploration, feature engineering, model training, and a simple app for credit risk checking.

## Project Structure
- `credit_check.ipynb`: Main notebook for data analysis, visualization, and modeling.
- `german_credit_data.csv`: Dataset containing customer credit information.
- `app.py`: Example script for risk prediction (can be adapted for Streamlit or other apps).

## Main Steps
1. **Data Exploration**: Visualize and summarize the dataset, check for missing values and outliers.
2. **Feature Engineering**: Encode categorical variables, handle missing data, and prepare features for modeling.
3. **Model Training**: Train Decision Tree, Random Forest, Extra Trees, and XGBoost models. Use GridSearchCV for hyperparameter tuning.
4. **Evaluation**: Compare model performance and select the best model.
5. **Credit Check App**: Use the best model to predict credit risk for new data.

## How to Run

### Requirements
- Python 3.8+
- Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost joblib
```

### Steps
1. **Open the notebook**
   - Run `credit_check.ipynb` in Jupyter or VS Code.
   - Follow the cells step by step for data analysis and modeling.

2. **Run the app (optional)**
   - Adapt `app.py` for your use case (e.g., Streamlit web app).
   - Example (for Streamlit):
     ```bash
     pip install streamlit
     streamlit run app.py
     ```

## Notes
- The target variable is `Risk`: 1 = good (Lower Risk), 0 = bad (Higher Risk).
- The best model (Extra Trees) achieves ~0.69 accuracy.
- You can further improve the app or modeling as needed.

## Author
- Cigdem Akdemir

## License
MIT License
