# 🏠 Interpretable Home Risk

This project explores **credit risk modeling** using the Home Credit Default Risk dataset. It focuses on building a transparent, interpretable machine learning pipeline that balances predictive performance with real-world explainability.

🔍 All model outputs are translated into **interactive Tableau dashboards** for stakeholders.

🔗 **Tableau Dashboard**:  
[Loan Default Risk Analysis — Model Results, SHAP & Metrics](https://public.tableau.com/app/profile/saayed.alam/viz/LoanDefaultRiskAnalysisModelResultsSHAPMetrics/0-Overview)

---

## 📦 Dataset

- Source: [Kaggle – Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk)
- Size: ~150MB (not included in this repo due to size limits)
- Description: Includes financial, demographic, and credit history data for loan applicants.

---

## 🧠 Project Structure

| Folder / File | Purpose |
|---------------|---------|
| `notebooks/`  | Clean, modular Jupyter notebooks (EDA, modeling, SHAP, Tableau prep) |
| `models/`     | Saved trained LightGBM model |
| `data/processed/` | Cleaned and encoded data |
| `data/final/` | Tableau-ready CSV exports |
| `.gitignore`  | Ensures raw data and temp files are excluded from GitHub |
| `requirements.txt` | Python dependencies for reproducibility |

---

## 🎯 Key Goals

- Build a high-performing credit risk model (LightGBM)
- Ensure **interpretability** with SHAP values
- Segment results by **risk bands**
- Export visual-ready data for Tableau
- Share findings via an interactive dashboard

---

## 📊 Core Visualizations

1. **SHAP Global Importance**  
   - Feature-level impact rankings on model output  
2. **Risk Distribution by Ground Truth**  
   - Histogram of predicted scores by actual label  
3. **SHAP Aggregated by Risk Band**  
   - Top 15 features grouped by low, medium, high risk  
4. **SHAP vs. Risk Score**  
   - Scatter plots of feature impact vs. probability  
5. **Confusion Matrix & Metrics**  
   - Precision, recall, TP/FP/FN/TN breakdown  

---

## ⚙️ Setup Instructions

```bash
# Clone the repo
git clone git@github.com:saayedalam/interpretable-home-credit-risk.git
cd interpretable-home-credit-risk

# (Optional) Create a virtual environment
python3 -m venv jupyterlab-env
source jupyterlab-env/bin/activate

# Install dependencies
pip install -r requirements.txt

# Launch JupyterLab
jupyter lab
