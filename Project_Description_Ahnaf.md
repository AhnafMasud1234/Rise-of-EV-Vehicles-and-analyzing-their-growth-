# The Rise of Electric Vehicles: A Data-Driven Analysis Using IEA Global EV Data

## Executive Summary

This research project presents a comprehensive data analytics investigation into the global adoption of Electric Vehicles (EVs) utilizing historical data from the International Energy Agency (IEA). The study employs exploratory data analysis, statistical correlation methods, and regression modeling techniques to identify the key factors driving EV adoption worldwide and to forecast future growth trajectories through 2030.

## Research Objectives

The primary objectives of this analysis are to:

1. Examine the historical growth patterns of global EV adoption from 2010 to 2024
2. Identify and quantify the key factors contributing to the rise of electric vehicles
3. Evaluate the effectiveness of government policies across different countries and regions
4. Develop predictive models to forecast EV adoption trends through 2030
5. Provide data-driven insights for understanding the future of electric mobility

## Dataset Information

| Attribute | Description |
|-----------|-------------|
| **Source** | International Energy Agency (IEA) Global EV Data Explorer |
| **Coverage** | 2010 - 2024 |
| **Records** | 16,437 observations |
| **License** | Creative Commons Attribution 4.0 International (CC BY 4.0) |

### Variables Analyzed

- **EV Stock**: Cumulative number of electric vehicles in operation
- **EV Sales**: Annual electric vehicle sales volume
- **EV Sales Share**: Percentage of total vehicle sales represented by EVs
- **Charging Infrastructure**: Number of public charging points deployed
- **Oil Displacement**: Volume of oil consumption avoided due to EV adoption
- **Powertrain Distribution**: Market share comparison between BEV and PHEV technologies

## Methodology

### Data Preprocessing

The raw dataset underwent rigorous cleaning procedures including removal of projection-based records, elimination of duplicate entries, standardization of variable naming conventions, and conversion of data types to ensure analytical integrity.

### Analytical Framework

**Exploratory Data Analysis**: Comprehensive visualization of temporal trends, geographic distributions, and cross-variable relationships to establish foundational understanding of EV adoption patterns.

**Correlation Analysis**: Statistical examination of relationships between EV adoption indicators to identify interdependencies among market growth, infrastructure development, and environmental impact metrics.

**Regression Modeling**: Application of three regression approaches to model and predict EV adoption:

| Model | Predictor Variables | Purpose |
|-------|---------------------|---------|
| Simple Linear Regression | Year | Baseline trend estimation |
| Multiple Linear Regression | Year, Charging Infrastructure | Multi-factor influence assessment |
| Polynomial Regression (Degree 3) | Year (with polynomial terms) | Non-linear growth pattern capture |

### Model Evaluation

All models were assessed using standardized performance metrics:
- **R² Score**: Coefficient of determination measuring explanatory power
- **MAE**: Mean Absolute Error quantifying average prediction deviation
- **RMSE**: Root Mean Squared Error penalizing larger prediction errors

## Principal Findings

### Market Growth Dynamics

Global EV stock demonstrated exponential growth, expanding from fewer than 1 million vehicles in 2010 to exceeding 45 million in 2024, representing a 45-fold increase over the study period. Annual sales reached 17 million units in 2024, constituting approximately 20% of global vehicle sales.

### Critical Success Factors

The analysis identified five primary drivers of EV adoption:

1. **Government Policy Intervention**: Nations implementing comprehensive incentive programs (subsidies, tax exemptions, purchase mandates) demonstrate significantly higher adoption rates. Norway achieved greater than 90% EV sales share through sustained policy support initiated in the 1990s.

2. **Battery Cost Reduction**: Manufacturing cost decreases of approximately 87% between 2010 and 2023 have substantially improved EV affordability and market competitiveness.

3. **Charging Infrastructure Expansion**: Strong positive correlation (>0.95) between charging point availability and EV adoption confirms infrastructure as a critical enabler of market growth.

4. **Environmental Impact**: EVs displaced over 1 million barrels of oil daily in 2024, demonstrating measurable progress toward transportation sector decarbonization.

5. **Technology Maturation**: Battery Electric Vehicles (BEV) now command approximately 70% market share over Plug-in Hybrid Electric Vehicles (PHEV), reflecting consumer confidence in full electrification.

### Predictive Model Performance

| Model | R² Score | Interpretation |
|-------|----------|----------------|
| Simple Linear | ~0.85 | Systematic underestimation due to linear assumption |
| Multiple Linear | ~0.90 | Improved fit through infrastructure variable inclusion |
| **Polynomial (Degree 3)** | **~0.99** | **Superior fit capturing exponential growth dynamics** |

### Forecast Projections (2030)

Based on the optimal polynomial regression model:
- **Global EV Stock**: Projected to exceed 200 million vehicles
- **Annual EV Sales**: Projected to surpass 30 million units

## Repository Structure

```
├── README.md                           # Project documentation
├── EVDataExplorer2025.csv              # Source dataset (IEA)
├── Ahnaf_EV_Final.ipynb                # Complete analytical notebook
└── EV_Analysis_Report_Ahnaf.docx       # Formal research report
```

## Technical Requirements

### Software Dependencies

- Python 3.12 or higher
- Jupyter Notebook environment

### Required Libraries

```
pandas>=2.0.0
numpy>=1.24.0
matplotlib>=3.7.0
seaborn>=0.12.0
scikit-learn>=1.3.0
```

### Installation

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Execution Instructions

1. Clone this repository to your local environment
2. Ensure all dependencies are installed
3. Launch Jupyter Notebook and open `Ahnaf_EV_Final.ipynb`
4. Execute cells sequentially to reproduce the analysis

## Author

**Mohammad Ahnaf Masud**  
Schiller International University, Madrid Campus  
Course: CS430 - Data Analytics  
Instructor: Professor Dhaval Gadariya  
Academic Year: 2025-2026

## References

International Energy Agency. (2024). *Global EV Outlook 2024: Moving Towards Increased Affordability*. IEA Publications. https://www.iea.org/reports/global-ev-outlook-2024

International Energy Agency. (2025). *Global EV Outlook 2025: Expanding Sales in Diverse Markets*. IEA Publications. https://www.iea.org/reports/global-ev-outlook-2025

International Energy Agency. (2025). *Global EV Data Explorer*. IEA Data and Statistics. https://www.iea.org/data-and-statistics/data-tools/global-ev-data-explorer

## License

This project utilizes publicly available data from the International Energy Agency, distributed under the Creative Commons Attribution 4.0 International License (CC BY 4.0). Proper attribution to the IEA is maintained throughout this work.

---

*Repository Last Updated: January 2026*
