# Predicting and Explaining Digital Public Infrastructure Performance Across Indian States

**Course:** QM640 Data Analytics Capstone  
**Institution:** Walsh College  
**Student:** Nandini Nagaraj  
**Instructor:** Mr. Shyam Venkatesh  
**Term:** Fall 2025 Term 3  

---

## Project Overview

This project develops a supervised machine learning framework to classify Indian states and union territories as high-performing or low-performing on Digital Public Infrastructure (DPI) metrics, and to identify the key socio-economic and digital drivers of that performance.

**Digital Public Infrastructure** includes platforms such as Aadhaar (biometric identity), UPI (Unified Payments Interface), and DigiLocker — collectively known as the India Stack.

---

## Research Questions

| # | Research Question |
|---|---|
| RQ1 | Can states be classified into high/low performance categories using digital and socio-economic indicators? |
| RQ2 | What are the most important variables driving regional DPI performance? |
| RQ3 | How do logistic regression, random forest, and XGBoost compare in predictive performance? |
| RQ4 | Does a composite digital adoption index improve model accuracy and interpretability? |

---

## Repository Structure

```
dpi-capstone-qm640/
│
├── data/
│   ├── dpi_state_data.csv          # Main dataset (state-year level)
│   └── data_dictionary.md          # Variable definitions
│
├── notebooks/                      # To be added during project execution
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_modeling_rq1_rq2.ipynb
│   └── 04_modeling_rq3_rq4.ipynb
│
├── outputs/                        # Model results, charts (to be added)
│
├── synopsis/
│   └── QM640_Synopsis_Nandini_Nagaraj.pdf
│
└── README.md
```

---

## Dataset

- **Unit of analysis:** Indian state / union territory, by year
- **Time period:** 2019–2023
- **Observations:** ~160 (28 states × 5 years, with some UTs)
- **Target variable:** `performance_category` (1 = high-performing, 0 = low-performing)

### Data Sources

| Variable | Source | URL |
|---|---|---|
| UPI transactions per capita | NPCI | https://www.npci.org.in/what-we-do/upi/product-statistics |
| Internet penetration | TRAI | https://trai.gov.in |
| Aadhaar coverage | MeitY / UIDAI | https://uidai.gov.in |
| Literacy rate | Census of India | https://censusindia.gov.in |
| Per capita income | data.gov.in | https://data.gov.in |
| Urbanization rate | Census of India | https://censusindia.gov.in |

---

## Models Used

- Logistic Regression (baseline)
- Random Forest
- XGBoost

## Explainability

SHAP (SHapley Additive exPlanations) values will be used for global and local model interpretation.

---

## Requirements

```
python >= 3.9
pandas
numpy
scikit-learn
xgboost
shap
matplotlib
seaborn
jupyter
```

Install with:
```bash
pip install -r requirements.txt
```

---

## Status

- [x] Synopsis submitted
- [ ] Data collection and cleaning
- [ ] Exploratory data analysis
- [ ] Model training and evaluation
- [ ] Final report

---

## Contact

Nandini Nagaraj — Walsh College — QM640 Spring 2026
