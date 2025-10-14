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

## Feature Engineering Summary

| Feature               | Description                                                  |
|-----------------------|--------------------------------------------------------------|
| xG Difference          | Expected goals scored minus expected goals conceded          |
| Home Advantage         | Binary indicator for home team status                        |
| Average Goal Difference| Rolling average of goal difference over recent matches       |
| Form Streak            | Encoded win/loss/draw streak over last 5 games               |
| Head-to-Head Score     | Historical win ratio between competing teams                 |

## Model Performance
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


