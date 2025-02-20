# Backpack Price Prediction

A machine learning project leveraging advanced regression models to predict backpack prices based on multiple features.

## Project Overview

This project implements various machine learning algorithms to predict backpack prices using the following key features:

- Brand (Nike, Adidas, Puma, etc.)
- Material (Leather, Canvas, Nylon, etc.)
- Size (Small, Medium, Large)
- Number of Compartments
- Laptop Compartment (Yes/No)
- Waterproof (Yes/No)
- Style (Backpack, Messenger, Tote)
- Color
- Weight Capacity (kg)

## Dataset
Source: Kaggle's Playground Series - Season 5, Episode 2  
[Dataset Link](https://www.kaggle.com/competitions/playground-series-s5e2)

### Dataset Statistics
- Training Set: 3,694,318 samples × 11 features
- Test Set: 300,000 samples × 11 features

### Data Quality
Missing Values Analysis:
| Feature | Training Set | Test Set |
|---------|-------------|-----------|
| Color | 3.35% | 3.32% |
| Brand | 3.17% | 3.24% |
| Material | 2.78% | 2.78% |
| Size | 2.20% | 2.20% |
| Style | 2.60% | 2.66% |
| Others | <3% | <3% |

## Models Implemented
- Random Forest Regressor
- XGBoost Regressor
- LightGBM Regressor
- CatBoost Regressor
- Neural Network

## Feature Engineering

### Created Features
- Brand-Material Interaction
- Brand-Size Interaction
- Weight Capacity Ratio
- Weight-to-Compartments Ratio
- Style-Size Interaction
- Binary Features:
    - Laptop Compartment
    - Waterproof
- Compartment Categories (Few, Moderate, Many, Too Many)

## Model Performance
Best Performing Model: LightGBM
- Validation RMSE: 39.015746
- Validation R²: 0.001205

## Usage
1. Clone the repository

```bash
git clone https://github.com/Shashank-143/Backpack-Price-Prediction.git
```

2. Install dependencies
```bash
pip install -r requirements.txt
```
3. Launch Jupyter notebook:
```bash
jupyter notebook "Backpack Price Prediction.ipynb"
```

## Acknowledgments
- Kaggle - Dataset provider
- Open-source ML library maintainers