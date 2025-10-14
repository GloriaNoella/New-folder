# Premier League Match Outcome Predictions

## About the Project
This repository presents a machine learning pipeline for predicting Premier League match outcomes using engineered features derived from historical performance data. The project is designed to demonstrate the strategic application of data science in sports analytics, with a focus on reproducibility, feature engineering, and stakeholder engagement

## Objectives
- Build a predictive model for Premier League match outcomes
- Engineer impactful features such as xG difference, home advantage, and recent form
- Visualize performance metrics and feature importance
- Translate model outputs into digital content for public engagement

## Technical Stack
- **Language**: Python
- **Libraries**: scikit-learn, pandas, NumPy, matplotlib, seaborn
- **Environment**: Jupyter Notebooks
- **Version Control**: Git & GitHub
  
## Data Sources

This project utilizes match data from **six Premier League seasons**, stored as structured CSV files. Each file contains team performance metrics, match outcomes, and features engineered for predictive modeling.

### Season Mapping Convention
To maintain consistency across multi-year datasets, each season is saved using a shorthand identifier based on the end year:

| Season         | File Name             |
|----------------|-----------------------|
| 2020/2021      | `PL Season 2021.csv`  |
| 2021/2022      | `PL Season 2122.csv`  |
| 2022/2023      | `PL Season 2223.csv`  |
| 2023/2024      | `PL Season 2324.csv`  |
| 2024/2025      | `PL Season 2425.csv`  |
| 2025/2026      | `PL Season 2526.csv`  |

All files are stored in the `/data` directory and are preprocessed for feature engineering and model input. This naming convention simplifies version control, model training workflows, and future scalability.

### Data Consolidation
To streamline preprocessing and model training, all six season files were **merged into a single master dataset**. This unified file enables:
- Consistent feature engineering across seasons
- Scalable model training and evaluation
- Simplified data access for reproducibility

## Feature Engineering Summary

| Feature               | Description                                                  |
|-----------------------|--------------------------------------------------------------|
| xG Difference          | Expected goals scored minus expected goals conceded          |
| Home Advantage         | Binary indicator for home team status                        |
| Average Goal Difference| Rolling average of goal difference over recent matches       |
| Form Streak            | Encoded win/loss/draw streak over last 5 games               |
| Head-to-Head Score     | Historical win ratio between competing teams                 |

##  xG Regression Modeling
Model Performance is as follows:
- **Accuracy**: 72% on validation set
- **F1 Score**: 0.68 (balanced across classes)
- **Evaluation Metrics**: Confusion matrix, ROC curve, precision-recall analysis

## Content Strategy
Model predictions are repurposed into short-form video content featuring:
- Visual breakdowns of match predictions
- Commentary on feature impact
- Audience engagement polls
- Post-match performance reviews

## How to Run Locally
```bash
git clone https://github.com/GloriaNoella/pl-predictions.git
cd pl-predictions
pip install -r requirements.txt
jupyter notebook

## Repository Structure
pl-predictions/
├── data/                  # Raw and processed datasets
├── notebooks/             # Jupyter notebooks for EDA and modeling
├── scripts/               # Python scripts for feature engineering and training
├── visuals/               # Plots and visual assets for content
├── README.md              # Project overview and documentation
├── requirements.txt       # Python dependencies


