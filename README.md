# 🌍 Global Obesity & Diet Visualisation

An interactive data visualisation storyboard exploring how macronutrient intake
shapes the global obesity crisis — built in R for MATH2270 (Data Visualisation
and Communication) at RMIT University.

## 📊 Live Project

👉 [View on RPubs](http://rpubs.com/Prathibha23/1321008)

## 🔍 Overview

This project investigates the relationship between dietary patterns and obesity
rates across 5,600+ country-year observations from 1990 to 2022.

Key questions explored:
- How have global macronutrient intakes shifted over three decades?
- Which nutrients are most strongly linked to rising obesity rates?
- Can we predict obesity rates from diet alone?

## 📈 Visualisations

- **Stacked area chart** — global macronutrient intake trends (1990–2022)
- **Line chart** — global average obesity rate over time
- **Correlation heatmap** — macronutrients vs. obesity rate
- **Scatter plots** — obesity vs. each macronutrient (sugar, fat, carbs, protein)
- **Bar chart** — top 10 countries by average obesity rate
- **Regression plot** — predicted vs. actual obesity rates

## 🗂️ Data Sources

| Dataset | Source |
|---|---|
| Obesity prevalence (BMI ≥ 30) | [WHO GHO via Our World in Data](https://ourworldindata.org/grapher/obesity-prevalence-adults-who-gho) |
| Dietary composition by country | [FAO via Our World in Data](https://ourworldindata.org/grapher/dietary-composition-by-country) |
| Daily caloric supply (macronutrients) | [Our World in Data](https://ourworldindata.org/grapher/daily-caloric-supply-derived-from-carbohydrates-protein-and-fat) |

## 🛠️ Libraries Used

```r
library(dplyr)
library(ggplot2)
library(tidyr)
library(plotly)
library(readr)
library(patchwork)
```

## 💡 Key Findings

- Global obesity more than doubled from ~10% (1990) to over 23% (2022)
- Sugar and fat intake show the strongest positive correlation with obesity
- Plant-based diets appear to offer a modest protective effect
- Pacific island nations (Tonga, Nauru, Tuvalu) have the highest average obesity rates
- A multiple regression model using all macronutrients explains ~37% of obesity variance (R² = 0.37)
