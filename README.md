
# Electric Vehicle (EV) Adoption Analysis & Forecasting

This project investigates electric vehicle adoption patterns across the United States, leveraging machine learning and statistical techniques to analyze and forecast EV trends. The study uses the Electric Vehicle Population Dataset and combines data preprocessing, exploratory data analysis, predictive modeling, and policy simulation.

## Project Overview

The project explores:

- Key factors influencing EV adoption (e.g., electric range, MSRP)
- Manufacturer-wise adoption rates and state-level penetration
- Predictive modeling (Linear Regression, Random Forest, ARIMA)
- Policy simulation to evaluate adoption growth scenarios

## Dataset

- Source: data.wa.gov – Electric Vehicle Population Dataset
- Time Range: 2010–2023
- Records: ~1.2 million EV registrations across U.S. states
- Key Features: Make, Model, Model Year, Electric Range, MSRP, EV Type, State, Registration Date

## Key Methods

### Data Preprocessing

- Handled missing values for Electric Range, Base MSRP, and Electric Utility
- Added a Year column for temporal trend analysis
- Standardized inconsistent categorical data

### Exploratory Data Analysis

- Distribution of EV types (BEV vs PHEV)
- Histogram and KDE plots for electric range
- Year-wise trend line of EV registrations
- Top EV manufacturers (Tesla, Chevrolet, Nissan, etc.)
- Correlation heatmap to identify key predictors

### Machine Learning Models

| Model                | Task                  | Key Metric       | R² Score |
|----------------------|------------------------|------------------|----------|
| Linear Regression    | Predict Electric Range | MAE, MSE          | 0.92     |
| Random Forest        | Predict Electric Range | MAE, MSE          | 0.96     |
| ARIMA (Time Series)  | Forecast EV Adoption   | Forecast Accuracy | 0.89     |

### Forecasting

- ARIMA model used to forecast EV registrations through 2028
- Forecast volatility increases over time; suitable for short-term projections

### Policy Simulation

- Modeled a 50% post-2020 policy-driven increase in EV adoption
- Visualized impact showing accelerated adoption trajectory

## Key Findings

- Electric Range is the strongest predictor of adoption (importance: 0.82)
- Tesla leads EV market with 42% share
- EV adoption is heavily urban-centric (82.4% of registrations)
- Policy incentives significantly accelerate adoption (up to 58% by 2025)
- ARIMA models are useful for near-term projections but lose accuracy over time

## Visualizations

Featured plots:

- EV Adoption Over Time
- Electric Range Distribution
- Top 10 EV Manufacturers
- EV Type Breakdown
- Correlation Heatmap
- Actual vs. Predicted (Random Forest)
- ARIMA Forecast
- Policy Simulation Comparison
- EV Adoption by State

All visualizations are included in the notebook with professional design and intuitive color palettes.

## Project Structure

```
.
├── Electric_Vehicle_1.ipynb        # Main Jupyter Notebook
├── Electric_Vehicle_Population_Data.csv  # Input dataset
├── README.md                       # Project summary and documentation
└── report/
    └── Nasir Report final_updated.docx   # Full project report
```

## Skills Applied

- Python (pandas, seaborn, matplotlib, sklearn, statsmodels)
- Data wrangling and feature engineering
- Statistical analysis and EDA
- Machine learning regression
- Time series forecasting (ARIMA)
- Data visualization
- Policy modeling and simulation

## References

- Pojani et al., 2021 - Transport, Gender, and Culture
- Sierzchula et al., 2014 - Financial Incentives and Socio-Economic Factors
- Khan and Wyrwa, 2024 - Quantitative Techniques in Electricity Consumption Forecasting
- IEA, 2023 - Global EV Outlook

## Author

Nasir – MSc Data Science Final Project  
University of Hertfordshire  

