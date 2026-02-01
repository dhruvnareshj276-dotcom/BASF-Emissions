# BASF Emissions ML & ESG Text Analysis

This repository contains a two-part sustainability analytics project:

##  Task 1 — Emission Prediction Using Machine Learning

We use the EDGAR CO₂ emissions dataset to predict future emissions trends using historical data.

### Models Used
- Ridge Regression (Linear baseline)
- Random Forest Regressor (Nonlinear model)

### Evaluation Metrics
- RMSE
- MAE
- R²

### Outputs
- Actual vs Predicted Emissions Plot
- Feature Importance Plot

---

##  Task 2 — ESG Commitment Extraction (NLP)

This task automatically extracts emission-reduction commitments from a sustainability report PDF.

### Steps
1. Extract text from PDF using `pdfplumber`
2. Clean text (lowercase, remove punctuation)
3. Identify emission-related sentences using:
   - Keyword rules
   - TF-IDF scoring
4. Extract commitment statements (e.g., "Reduce emissions by 25% by 2030")

---

## Data Sources

- EDGAR CO₂ Dataset:  
  https://github.com/openclimatedata/edgar-co2-emissions

- BASF Sustainability Report:  
  https://report.basf.com/2024/en/services/downloads.html

---

##  How to Run

```bash
pip install -r requirements.txt
python task1_emission_prediction.py

python task2_commitment_extraction.py

