# Predicting Fraudulent Insurance Claims Using Machine Learning 

This project builds a supervised ML pipeline to detect fraudulent insurance claims using models like XGBoost, Random Forest, SVM, and Logistic Regression. It includes data preprocessing, feature engineering, model evaluation, SHAP explainability, and MLflow experiment tracking.

---

## Objective

To help insurance providers automatically flag potentially fraudulent claims for review, reducing financial loss and manual effort.

---

## Features

- Data profiling and preprocessing (handling missing values, encoding, scaling)
- Feature engineering (claim ratios, time bins)
- Model training & comparison (XGBoost, Random Forest, SVM, Logistic Regression)
- MLflow tracking for metrics, parameters, and artifacts
- SHAP visualizations for interpretability
- Confusion matrix, ROC curves, and F1-score comparisons

---

## Usage

1. **Clone the Repository**

```bash
git clone https://github.com/Fatimat01/insurance-fraud-prediction.git
cd insurance-fraud-detection
```
2. **Install Dependencies**
```bash
pip install -r requirements.txt
```

3. **Launch MLflow UI**

```bash
mlflow ui
```

4. **Run Notebooks**

- `notebooks/data-processing.ipynb` – for preprocessing and feature selection
- `notebooks/model-train.ipynb` – for training and MLflow logging


Open your browser at [http://localhost:5000](http://localhost:5000) to view the MLflow UI.

---

## Project Structure

```text
.
├── data
│   ├── fraud_claims.csv
│   ├── processed_insurance_data.csv
│   └── selected_features.csv
├── mlartifacts/               # MLflow-exported model artifacts, visualizations & SHAP plots
├── mlruns/                    # MLflow tracking metadata (experiments, metrics, params)
├── notebooks/
│   ├── data-processing.ipynb              # Preprocessing, encoding, and scaling
│   └── model-train.ipynb                  # Training, evaluation, logging
├── reports/
│   └── data_profile.html      # Data profiling report (ydata-profiling)
├── README.md                   # You are here!

```

---

## Model Evaluation Summary

| Model           | Accuracy | Recall | Precision | AUC   | F1-Score |
|----------------|----------|--------|-----------|-------|----------|
| XGBoost         | 0.85     | 0.65   | 0.71      | 0.828 | 0.68     |
| Random Forest   | 0.835    | 0.816  | 0.625     | 0.826 | 0.707    |
| SVM             | 0.705    | 0.755  | 0.44      | 0.820 | 0.556    |
| Logistic Reg.   | 0.68     | 0.796  | 0.419     | 0.815 | -        |

---

## Contributors

- **Fatimat Atanda**
- **Robair Farag**
- **Jacob Edwards**

---

## License

This project is licensed under the MIT License.