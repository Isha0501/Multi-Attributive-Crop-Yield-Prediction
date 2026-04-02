# 🌽 Multi-Attributive Crop Yield Prediction

**Published in IEEE Xplore** · [Read the Paper](https://ieeexplore.ieee.org/document/11253730)
---

## The Problem

Global food demand is rising — but a surprising amount of agricultural produce never makes it to consumers, not because it wasn't grown, but because supply chains lack the forecasting tools to manage it well. Accurate crop yield prediction is a foundational fix for that, yet most existing approaches rely on limited public datasets and treat all features as equally important. We wanted to do better.

## What We Built

A custom-curated maize yield dataset built by integrating three data sources — **Kaggle**, **data.gov.in**, and **NRSC** — aligned through a rainfall-based correlation methodology. This gave us a richer, more granular view of the soil and environmental factors that actually drive yield outcomes.

We then benchmarked four ML models across this dataset:

| Model | Notes |
|---|---|
| 🌲 Random Forest | **Best performer — 95.5% R²** |
| ⚡ XGBoost | Strong baseline |
| 🐱 CatBoost | Robust on categorical features |
| 📐 SVR | Classical regression benchmark |

Evaluation used MAE, MSE, RMSE, and R² across multiple attribute sets, with variable importance analysis to understand *what* is actually driving predictions.

## Key Takeaway

Random Forest outperformed all models at 95.5% R² — but the more interesting finding was how much the *dataset construction* mattered. Custom multi-source integration consistently outperformed models trained on single public datasets, validating that the data pipeline is just as important as the model choice.
