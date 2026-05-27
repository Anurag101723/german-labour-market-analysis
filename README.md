# 🇩🇪 German Labour Market Analysis 2012–2021

> Analysis of German unemployment trends using official Bundesagentur für Arbeit data — uncovering regional disparities, East vs West Germany differences, COVID-19 impact, and occupation-level insights across 401 districts and 145 occupational groups.

![Python](https://img.shields.io/badge/Python-3.12-blue?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-orange?style=flat&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat)
![Data](https://img.shields.io/badge/Data-Bundesagentur%20für%20Arbeit-black?style=flat)

---

## 📌 Overview

Germany's labour market is one of the most closely watched in Europe. This project analyses **10 years of official unemployment data** from the Bundesagentur für Arbeit (Federal Employment Agency) — covering 401 German districts, 145 occupational groups, and the full impact of COVID-19 on the German workforce.

The analysis uncovers structural disparities between East and West Germany, identifies the most vulnerable occupational groups, and quantifies the COVID-19 shock on regional labour markets.

---

## 🎯 Key Findings

| Finding | Insight |
|---|---|
| National improvement | Unemployment fell **15.7%** from 2012 to 2019 |
| COVID-19 shock | **+18.4% spike** in unemployment in 2020 alone |
| East Germany | **−26%** unemployment reduction 2012–2021 |
| West Germany | **+7%** unemployment increase 2012–2021 |
| Hardest hit sector | Road Transport & Logistics (+highest COVID impact) |
| Most resilient | Social Work, Education, Care sectors |
| Biggest state | NRW dominates West Germany unemployment totals |

---

## 📊 Dataset

- **Source:** Bundesagentur für Arbeit via [Zenodo — badata package](https://zenodo.org/records/7664361)
- **Period:** 2012 – 2021
- **Coverage:** 401 German districts (Kreise)
- **Occupations:** 145 occupational groups
- **Records:** 568,480 observations
- **Variables:** Region, Occupational Group, Year, Total Unemployed, Women Unemployed

---

## 🔍 Analysis Sections

**1. National Unemployment Trend**
- 7 years of continuous improvement (2012–2019)
- COVID-19 shock clearly visible in 2020
- Recovery trajectory in 2021

**2. State-Level Analysis**
- Unemployment breakdown across all 16 German states
- NRW identified as dominant contributor to West Germany totals
- Women % of unemployed by state

**3. East vs West Germany**
- East Germany reduced unemployment by 26% — structural investment paying off
- West Germany more exposed to COVID due to service sector concentration
- Ruhr area (NRW) driving West Germany's structural unemployment

**4. Occupation Analysis**
- Top unemployed occupations: Logistics, Sales, Cleaning, Office/Secretarial
- All top roles share common risk factors: low skill, automation exposure
- COVID impact measured per occupation (2019 vs 2020 % change)

**5. Policy Recommendations**
- Reskilling priority for logistics and warehouse workers
- Apply East Germany success model to high-unemployment West regions
- Gender-neutral retraining programmes across all 16 states

---

## 🛠️ Tech Stack

- **Language:** Python 3.12
- **Data Loading:** pyreadr (R data format conversion)
- **Data Processing:** Pandas, NumPy
- **Visualisation:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

---

## 🔍 Methodology

```
Bundesagentur für Arbeit Official Data (.rda format)
                ↓
Data Loading & Conversion
(pyreadr → Pandas DataFrames)
                ↓
Data Merging
(unemployment + region names + occupation names)
                ↓
State Classification
(16 German states + East/West mapping)
                ↓
Exploratory Data Analysis
(national trend, state breakdown, occupations, gender)
                ↓
East vs West Comparison
(% change analysis, COVID impact comparison)
                ↓
Occupation Trend Analysis
(COVID impact by sector, 2012-2021 trends)
                ↓
Policy Recommendations
```

---

## 📁 Repository Structure

```
german-labour-market-analysis/
│
├── german_labour_market.ipynb     # Main analysis notebook
├── README.md                      # Project documentation
```

> **Data Note:** The `.rda` dataset files are not included due to size.
> Download from: [Zenodo — badata v0.1.3](https://zenodo.org/records/7664361)

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/Anurag101723/german-labour-market-analysis.git
cd german-labour-market-analysis
```

2. Download dataset from Zenodo and extract to project folder
```
https://zenodo.org/records/7664361
```

3. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn pyreadr
```

4. Open the notebook
```bash
jupyter notebook german_labour_market.ipynb
```

---

## 👤 Author

**Anurag Rathore**
M.Sc. Big Data & Business Analytics — FOM University of Applied Sciences
📧 anuragakrathore@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/anurag1017) · [Portfolio](https://Anurag101723.github.io)
