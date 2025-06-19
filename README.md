# 📉 Financial Crises, Exchange Rate Volatility, and Socioeconomic Impact

> A Machine Learning Framework for Early Warning Systems in Global Financial Stability  
> **Authors**: Rohith Reddy Jonnalagadda, Allu Sagarika, Valluru Anjula Chakravarthy  
> **Affiliation**: University of North Texas  
> **Advisor**: Dr. Sam Shamroukh

---

## 📌 Abstract

This project investigates the early detection of financial crises — banking, currency, and systemic — using machine learning and macroeconomic indicators. We utilize a merged dataset combining the **Reinhart-Rogoff Global Crisis Dataset** and **IMF macroeconomic indicators** for 70 countries between 1980–2016. 

Our best-performing model, **XGBoost**, demonstrated superior accuracy in predicting systemic and inflation-related crises. The project underscores the utility of AI tools in macroeconomic forecasting and crisis prevention, offering potential support for global financial policy decisions.

---

## 🎯 Project Objectives

- Identify macroeconomic signals preceding financial crises.
- Evaluate the impact of **USD exchange rate volatility** on global stability.
- Develop and compare multi-output classification models.
- Recommend machine learning methods for real-time financial crisis monitoring.

---

## 📁 Current Repository Structure

```
├── financial_crisis_analysis.ipynb    # Main notebook containing EDA, feature engineering, modeling, and results()
└── README.md                          # Project documentation
```

> Additional scripts and datasets used during development are not included in this public version.

---

## 🧠 Methodology Summary


- **Data Sources**:
  - Reinhart-Rogoff Crisis Data (1800–Present)
  - IMF World Economic Outlook Data (1980–2016)

- **Data Preprocessing**:
  - Missing data handled via **MICE (Multiple Imputation by Chained Equations)**
  - Normality tested with **Shapiro-Wilk**
  - Multicollinearity checked via **VIF**
  - Non-parametric tree-based models chosen due to non-linearity

- **Modeling**:
  - Multi-output classifiers: `XGBoost`, `Random Forest`, `K-Nearest Neighbors (KNN)`
  - Evaluation using Accuracy, Precision, Recall, F1-Score

---

## 📊 Key Results

| Model         | Banking Crisis | Currency Crisis | Systemic Crisis |
|---------------|----------------|------------------|------------------|
| **XGBoost**   | 86% accuracy   | 86% accuracy     | **91% accuracy** |
| Random Forest | 83% accuracy   | 87% accuracy     | 89% accuracy     |
| KNN           | 78% accuracy   | 81% accuracy     | 86% accuracy     |

> Inflation crises were excluded from final conclusions due to perfect accuracy (100%) indicating likely data leakage or overfitting.

---

## 📌 Key Insights

- Exchange rate volatility and sovereign debt exposure are crucial leading indicators.
- USD appreciation often triggers financial tightening and crisis vulnerability.
- Crises are **not exclusive to developing economies** — developed countries are also at risk.
- Ensemble models outperform distance-based classifiers in handling macroeconomic data.

---

## 🧰 Tech Stack

| Tool/Library       | Purpose                          |
|--------------------|----------------------------------|
| Python             | Core programming language        |
| Pandas, NumPy      | Data handling                    |
| SciPy, Scikit-learn| Statistics, ML models            |
| XGBoost            | Gradient boosting classification |
| Matplotlib, Seaborn| Visualization                    |
| R (Tidyverse)      | Supplementary statistical tests  |

---

## ❓ Research Questions

- Can macroeconomic variables serve as early-warning indicators?
- How do exchange rate and inflation behave prior to crises?
- What is the role of USD dominance in global instability?
- Are ensemble models effective in forecasting multiple crisis types?

---

## 🔮 Future Directions

- Use **higher-frequency data** (monthly/quarterly) to improve sensitivity.
- Introduce **time-aware models** (LSTM, Transformer).
- Incorporate **market sentiment/news-based data**.
- Cluster countries based on economic characteristics for tailored models.

---

## 📄 Citation

```
@unpublished{chakravarthy2025crisisML,
  title={Financial Crises, Exchange Rate Volatility, and Socioeconomic Impact},
  author={Valluru Anjula Chakravarthy, Rohith Reddy Jonnalagadda, Allu Sagarika},
  year={2025},
  institution={University of North Texas}
}
```

---

## 🙏 Acknowledgements

Special thanks to **Dr. Sam Shamroukh** for mentorship, and to peers **Raahul Raj Akula** and **Bhavana Raj Rayapudi** for their support during this research.

