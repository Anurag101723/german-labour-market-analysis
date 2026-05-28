# German Labour Market Analysis 2012-2021

Analysis of unemployment trends using official Bundesagentur fur Arbeit data across 401 German districts, 145 occupational groups, and 10 years of records.

---

## Overview

Germany's labour market is one of the most closely watched in Europe. This project analyses 568,480 official unemployment records from the Bundesagentur fur Arbeit (Federal Employment Agency), covering the full period from the post-financial crisis recovery through the COVID-19 shock of 2020.

The analysis uncovers structural disparities between East and West Germany, identifies the most vulnerable occupational groups, quantifies the COVID-19 impact on regional labour markets, and delivers policy recommendations grounded in data.

---

## Dataset

| Property | Value |
|---|---|
| Source | Bundesagentur fur Arbeit via Zenodo (badata v0.1.3) |
| Period | 2012 to 2021 |
| Districts | 401 German Kreise |
| Occupational groups | 145 |
| Records after cleaning | 568,480 |
| Variables | Region, Occupational Group, Year, Total Unemployed, Women Unemployed |

Download: https://zenodo.org/records/7664361

---

## Key Findings

| Finding | Detail |
|---|---|
| National improvement 2012-2019 | Unemployment fell 15.7% over 7 years of economic growth |
| COVID-19 shock | 18.4% spike in unemployment in 2020 alone |
| East Germany 2012-2021 | 26% reduction in unemployment |
| West Germany 2012-2021 | 7% increase in unemployment |
| Hardest hit by COVID | Road transport and logistics |
| Most resilient sectors | Social work, education, care |
| Largest state contributor | NRW dominates West Germany unemployment totals |

---

## National Unemployment Trend

| Year | Total Unemployed | Change vs Previous Year |
|---|---|---|
| 2012 | 2,676,673 | Baseline |
| 2013 | 2,909,520 | +8.7% |
| 2014 | 2,875,345 | -1.2% |
| 2015 | 2,754,006 | -4.2% |
| 2016 | 2,666,431 | -3.2% |
| 2017 | 2,520,187 | -5.5% |
| 2018 | 2,297,767 | -8.8% |
| 2019 | 2,257,047 | -1.8% (pre-COVID low) |
| 2020 | 2,673,991 | +18.4% (COVID shock) |
| 2021 | 2,588,726 | -3.2% (recovery begins) |

---

## East vs West Germany

| Region | Change 2012-2021 | Interpretation |
|---|---|---|
| East Germany | -26% | Structural investment paying off. Started from higher base |
| West Germany | +7% | Greater service sector exposure to COVID lockdowns |

West Germany's higher COVID impact is partly explained by NRW, Germany's most populous state, which has structural unemployment in the Ruhr area from decades of deindustrialisation.

---

## Top Unemployed Occupations (2012-2021 Total)

| Rank | Occupation | Total Unemployed |
|---|---|---|
| 1 | Logistics, Warehouse, Post, Delivery | 2,336,074 |
| 2 | Sales (non-specialised) | 2,308,878 |
| 3 | Cleaning | 2,250,117 |
| 4 | Office and Secretarial | 1,885,924 |

All top occupations share common risk factors: low skill requirements, high volume, and significant automation exposure.

---

## COVID-19 Impact by Occupation (2019 to 2020)

| Occupation | Direction | Interpretation |
|---|---|---|
| Road Transport | Increase | Supply chain disruptions and mobility restrictions |
| Logistics and Warehouse | Increase | Factory shutdowns reduced goods movement |
| Sales | Increase | Retail closures during lockdowns |
| Cleaning | Increase | Office and hospitality closures |
| Social Work | Stable | Essential service, protected from COVID impact |
| Education and Care | Stable | Essential service, maintained demand |

---

## Policy Recommendations

| Area | Recommendation |
|---|---|
| Reskilling | Logistics and warehouse workers face both COVID vulnerability and automation risk. Targeted reskilling programmes are a priority |
| East Germany model | 26% reduction demonstrates structural interventions work. Apply learnings to high-unemployment West regions such as the Ruhr area |
| COVID resilience | Future crisis planning should prioritise protecting service sectors not classified as essential |
| Gender | Women represent 45-50% of unemployed consistently. Gender-neutral retraining programmes needed across all 16 states |
| Regional targeting | NRW, Berlin, and Sachsen-Anhalt require the most federal employment support |

---

## Methodology

```
Bundesagentur fur Arbeit Official Data (.rda format)

Data Loading
pyreadr converts R data files to Pandas DataFrames

Merging
Unemployment records joined with region names and occupation names

State Classification
16 German states mapped from 2-digit region codes
East and West Germany classification applied

Exploratory Data Analysis
National trend, state breakdown, occupations, gender share

East vs West Comparison
Percentage change analysis, COVID impact comparison

Occupation Trend Analysis
COVID impact by sector, 2012-2021 trends

Policy Recommendations
Based on structural findings and regional disparities
```

---

## Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3.12 |
| Data Loading | pyreadr |
| Data Processing | Pandas, NumPy |
| Visualisation | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |

---

## Repository Structure

```
german-labour-market-analysis/
|
|-- german_labour_market.ipynb
|-- README.md
```

Dataset files (.rda) not included. Download from Zenodo link above.

---

## How to Run

```bash
git clone https://github.com/Anurag101723/german-labour-market-analysis.git
cd german-labour-market-analysis
pip install pandas numpy matplotlib seaborn pyreadr
jupyter notebook german_labour_market.ipynb
```

---

## Author

Anurag Rathore  
anuragakrathore@gmail.com  
linkedin.com/in/anurag1017  
anurag101723.github.io
