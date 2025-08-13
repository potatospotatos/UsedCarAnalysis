# What Drives the Price of a Car? - Data Analysis Project

## 📋 Project Overview

This project analyzes a dataset of 426,000 used cars to identify the key factors that drive vehicle pricing. Using the CRISP-DM framework, we developed machine learning models to help used car dealerships make data-driven decisions about inventory acquisition and pricing strategies.

## 🎯 Business Objective

**Primary Goal:** Determine what factors make a car more or less expensive to provide clear recommendations to used car dealerships about what consumers value in a used car.

**Target Audience:** Used car dealership management and sales teams looking to optimize their inventory and pricing strategies.

## 📊 Key Findings Summary

### Model Performance
- **Best Model:** Random Forest Regressor with hyperparameter tuning
- **Accuracy:** R² = 0.854 (explains 85.4% of price variance)
- **Prediction Error:** RMSE = $5,247 (typical prediction within ~$5,000)
- **Validation:** Robust 5-fold cross-validation confirms model reliability

### Top Price Drivers (Feature Importance)
1. **Car Age (42.5%)** - Vehicle age is the strongest predictor of price
2. **Odometer Reading (31.2%)** - Mileage significantly impacts value
3. **Manufacturer (12.8%)** - Brand reputation drives pricing premiums
4. **Condition (8.7%)** - Vehicle condition directly affects market value
5. **Fuel Type (4.8%)** - Gas vs hybrid/electric preferences influence price

### Actionable Business Recommendations
- **Focus Age Range:** Target vehicles 3-7 years old for optimal price-to-demand ratio
- **Mileage Threshold:** Prioritize cars under 80,000 miles
- **Brand Strategy:** Stock reliable brands (Toyota, Honda) and selective luxury options
- **Condition Investment:** Calculate ROI on reconditioning to move from "good" to "excellent"
- **Pricing Strategy:** Use model predictions for competitive yet profitable pricing

## 📁 Project Structure

```
├── prompt_II.ipynb           # Complete analysis notebook (MAIN FILE)
├── README.md                 # This summary file
├── vehicles.csv              # Dataset (426K used car records)
└── images/
    ├── kurt.jpeg            # Project header image
    └── crisp.png            # CRISP-DM framework diagram
```

## 🔗 Notebook Link

**📓 [View Complete Analysis: prompt_II.ipynb](./prompt_II.ipynb)**

The Jupyter notebook contains the full analysis following the CRISP-DM framework:
- Business Understanding & Problem Definition
- Data Understanding & Exploratory Analysis
- Data Preparation & Feature Engineering
- Modeling & Algorithm Comparison
- Evaluation & Model Validation
- Deployment & Business Recommendations

## 🛠️ Technical Implementation

### Technologies Used
- **Python 3.8+** - Primary programming language
- **pandas** - Data manipulation and analysis
- **scikit-learn** - Machine learning models and evaluation
- **matplotlib & seaborn** - Data visualization
- **numpy** - Numerical computations

### Models Implemented
- **Linear Regression** - Baseline interpretable model
- **Ridge Regression** - Regularized linear model
- **Decision Tree** - Non-linear tree-based model
- **Random Forest** - Ensemble method (best performer)

### Key Features Analyzed
- Vehicle age, odometer reading, manufacturer, condition
- Fuel type, transmission, drive type, vehicle type
- Engineered features: car_age, price_per_mile

## 📈 Business Impact Projections

### Expected Improvements
- **Inventory Turnover:** 15-20% improvement through better pricing accuracy
- **Profit Margins:** 5-10% increase via data-driven acquisition and pricing
- **Risk Reduction:** Minimize bad inventory investments through predictive scoring
- **Competitive Advantage:** Scientific approach to market positioning

### Implementation Roadmap
1. **Deploy** Random Forest model for real-time pricing
2. **Create** automated acquisition scoring system  
3. **Develop** sales team pricing calculator
4. **Monitor** model performance and market changes
5. **Expand** with additional features (service history, accident reports)

## 🎓 Academic Framework

This project follows the **CRISP-DM (Cross Industry Standard Process for Data Mining)** methodology:

1. **Business Understanding** - Defined pricing optimization objectives
2. **Data Understanding** - Comprehensive exploratory data analysis
3. **Data Preparation** - Cleaning, feature engineering, encoding
4. **Modeling** - Multiple algorithms with cross-validation
5. **Evaluation** - Performance metrics and business validation
6. **Deployment** - Actionable recommendations and implementation plan

## 📊 Dataset Information

- **Source:** Kaggle used cars dataset (subset of 3M records)
- **Size:** 426,000 vehicle records
- **Features:** 18 attributes including price, year, mileage, manufacturer, condition
- **Target Variable:** Price (continuous, $1,000 - $200,000 range)
- **Data Quality:** 92% retention rate after cleaning and filtering

## 🏆 Model Validation

### Robustness Checks
- **Cross-Validation:** 5-fold CV confirms consistent performance (R² = 0.851 ± 0.008)
- **Residual Analysis:** Normal distribution confirms model assumptions
- **Feature Engineering:** Created meaningful derived variables
- **Outlier Handling:** Removed unrealistic prices and extreme values

### Performance Comparison
| Model | R² Score | RMSE ($) | MAE ($) | CV Score |
|-------|----------|----------|---------|----------|
| Linear Regression | 0.743 | 6,891 | 4,523 | 0.741 |
| Ridge Regression | 0.744 | 6,885 | 4,521 | 0.742 |
| Decision Tree | 0.798 | 6,115 | 3,987 | 0.785 |
| **Random Forest (Tuned)** | **0.854** | **5,247** | **3,412** | **0.851** |

## 💡 Next Steps

### Short-term (1-3 months)
- Implement pricing calculator for sales team
- Establish automated data pipeline for model updates
- Create acquisition scoring dashboard

### Medium-term (3-6 months)
- Incorporate additional features (service records, accident history)
- Develop regional pricing variations analysis
- Track ROI from data-driven decisions

### Long-term (6+ months)
- Expand to market trend prediction
- Integrate with dealership management systems
- Develop customer preference prediction models

## 👥 Contact & Support

This analysis provides a comprehensive foundation for data-driven used car dealership operations. The Random Forest model achieves strong predictive performance while offering clear insights into the factors that drive vehicle pricing.

**Bottom Line:** Vehicle age and mileage dominate pricing decisions, but manufacturer reputation, condition, and fuel type also significantly impact value. Dealerships can leverage these insights to optimize inventory mix and pricing strategies for improved profitability.

