# 📉 Financial Crises, Exchange Rate Volatility, and Socioeconomic Impact

> A Machine Learning Framework for Early Warning Systems in Global Financial Stability  
> **Authors**: Valluru Anjula Chakravarthy, Rohith Reddy Jonnalagadda, Allu Sagarika
> **Affiliation**: University of North Texas  
> **Advisor**: Dr. Sam Shamroukh

---

## 📌 Abstract

This project explores the development of an **early warning system** to forecast multiple types of financial crises—**banking**, **currency**, **systemic**, and **inflation**—using machine learning and macroeconomic indicators. By merging the **Reinhart-Rogoff Global Crisis dataset** with IMF economic data across **70 countries from 1980–2016**, the study applies multi-output classification models (XGBoost, Random Forest, KNN) to identify patterns and predictors of economic instability.

XGBoost achieved the best performance, particularly in forecasting **systemic and inflation crises**, demonstrating the feasibility of ensemble-based AI models in economic risk assessment. The research bridges **macroeconomic theory** with **modern machine learning**, paving the way for scalable, data-driven early warning systems.

---

## 📁 Project Structure

```
├── data/
│   └── merged_financial_dataset.csv
├── notebooks/
│   └── eda_and_modeling.ipynb
├── src/
│   ├── preprocessing.py
│   ├── models.py
│   └── evaluate.py
├── figures/
│   └── correlation_heatmap.png
├── report/
│   └── Project_Proposal_Draft.pdf
└── README.md
```

---

## 🎯 Objectives

- Analyze global financial crises (1980–2016) using economic indicators.
- Investigate the role of **USD exchange rate volatility** in global financial stability.
- Predict crisis occurrence using **multi-output classification models**.
- Provide policymakers and financial institutions with **early warning insights**.

---

## 🧠 Methodology

- **Data Sources**:
  - Reinhart-Rogoff Financial Crisis Dataset (1800–Present)
  - Macroeconomic Indicators from IMF

- **Target Variables**:
  - `Banking Crisis`, `Currency Crisis`, `Systemic Crisis`

- **Key Features**:
  - `GDP per capita`, `Exchange Rate (exch_usd)`, `Inflation Rate`, `Unemployment`, `Debt Defaults`, etc.

- **Preprocessing**:
  - Missing data handled using **MICE (Multiple Imputation by Chained Equations)**
  - Shapiro-Wilk test for normality
  - VIF for multicollinearity check

- **Models**:
  - ✅ XGBoost (Best performance)
  - ✅ Random Forest
  - ✅ K-Nearest Neighbors (baseline)

- **Evaluation Metrics**:
  - Accuracy, Precision, Recall, F1-Score

---

## 📊 Key Results

| Model         | Banking Crisis | Currency Crisis | Systemic Crisis |
|---------------|----------------|------------------|------------------|
| **XGBoost**   | 86% accuracy   | 86% accuracy     | **91% accuracy** |
| Random Forest | 83% accuracy   | 87% accuracy     | 89% accuracy     |
| KNN           | 78% accuracy   | 81% accuracy     | 86% accuracy     |

---

## 🔍 Visual Insights

- 📌 Correlation heatmap showing weak linearity → supports use of tree-based models.
- 🗺️ Country-wise banking crisis distribution: highest in Zimbabwe, Congo, and Central African Republic.
- 📈 Time series trends: crisis peaks in late 1990s and during 2008 Global Financial Crisis.

---

## 🧰 Tools & Libraries

| Tool/Library | Purpose |
|--------------|---------|
| **Python** | Main implementation language |
| Pandas, NumPy, SciPy | Data processing and assumption testing |
| Matplotlib, Seaborn | Data visualization |
| XGBoost, Scikit-learn | Machine Learning |
| R (tidyverse, dplyr) | Additional statistical analysis |
| SQL, Excel | Data wrangling |

---

## ❓ Research Questions

- What macroeconomic indicators serve as leading signals of financial crises?
- How do exchange rate fluctuations impact financial stability?
- Are developing economies more prone to currency crises?
- Can ensemble models predict multiple crisis types with high reliability?

---

## 🚀 Future Work

- Incorporate **quarterly/monthly data** for improved sensitivity.
- Apply **temporal models** like LSTMs or Transformers to capture lagged effects.
- Explore **sentiment analysis** using global news and investor confidence indices.
- Stratify models based on country clusters or economic zones.

---

## 📄 Citation

If you use this repository for your research, please cite:

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

We express deep gratitude to **Dr. Sam Shamroukh** for his mentorship, and to our peers **Raahul Raj Akula** and **Bhavana Raj Rayapudi** for their support during this research journey.
