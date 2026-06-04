# Multi-Perspective Analysis of COVID-19 Pandemic Dynamics

> A collaborative data analysis project examining pandemic dynamics through five complementary statistical lenses.

## Overview

This project provides an integrated analysis of the COVID-19 pandemic using WHO global data and World Bank socioeconomic indicators. Five research questions are addressed independently and synthesized into a unified narrative of how demographic, economic, and health system factors shaped pandemic outcomes across 167+ countries (2020–2022).

## Research Questions & Contributors

| # | Research Question | Method | Contributor |
|---|---|---|---|
| 1 | Exponential growth rates during the first wave (Türkiye, Italy, Germany) | Log-linear growth modeling | Hilal Görgülü |
| 2 | Socioeconomic determinants of first-wave peak severity | Regression & classification trees | Pelin Kımız |
| 3 | Health system mediation between socioeconomic factors and case outcomes | Multiple regression with interaction terms | Mert Değer |
| 4 | Mortality determinants: economic capacity vs. demographics | Multivariate regression | Ahmet Efe Gelibolu |
| 5 | Global temporal mortality trends (2020–2022) | Temporal & seasonal analysis | Nokwanele Pretty Gwebu |

## Key Findings

- **Türkiye** had the fastest early spread (31.1% daily growth, 2.23-day doubling time) despite its later pandemic onset compared to Italy and Germany
- **Population density** was the primary predictor of first-wave severity, with a classification tree achieving 79.2% accuracy in identifying high-risk countries
- **Physician density** showed a "surveillance paradox": better health systems both protect and increase detection, inflating reported CFRs in high-capacity countries
- **Age structure** (population 65+), not GDP, was the strongest predictor of COVID-19 mortality (β = 10.41, p < 0.001)
- **2021** was the deadliest year overall, accounting for ~54% of total pandemic mortality, despite 2022 recording higher single-day peaks (Omicron wave)

## Data Sources

- [WHO COVID-19 Database](https://covid19.who.int/) — Daily cases and deaths, 2020–2022
- [World Bank WDI](https://databank.worldbank.org/source/world-development-indicators) — GDP per capita, population age structure, physician density, urbanization, population density

## Methods & Tools

**Language:** R  
**Key packages:** `tidyverse`, `rpart`, `rpart.plot`, `patchwork`, `viridis`, `broom`  
**Statistical approaches:** Log-linear growth modeling, regression/classification trees, multiple linear regression with interaction terms, temporal decomposition

## Report

The full analysis is written in [Quarto](https://quarto.org/) (`.qmd`) and rendered as a self-contained HTML report with interactive code folding and a navigable table of contents.

To reproduce the report locally:
1- Install required packages
2- Render the report

> **Note:** The `WHO-COVID-19.csv` and `WDI.csv` data files must be placed in the same directory as `index.qmd` before rendering.

## Project Context

This project was completed as part of the **Concepts & Tools** course (CU-F25-MDSSB-01) at the university. All analyses were conducted independently per contributor and integrated into a single cohesive report.

## Authors

Ahmet Efe Gelibolu · Hilal Görgülü · Mert Değer · Nokwanele Pretty Gwebu · Pelin Kımız
