# User Event Funnel & Behavioral Risk Analysis

## Overview
This project analyzes user event data (app open → KYC → first transaction → credit application) to identify behavioral patterns that predict credit application completion.

**AUC Score:** 0.81

## Key Findings
- **23% drop-off at KYC stage** - the biggest leak in the funnel
- **Top 3 predictors of credit completion:**
  1. Median time between sessions (shorter = higher completion)
  2. Peak action velocity (bursts of activity = higher completion)
  3. Activity spike detection (unusual engagement = strong signal)

## Business Recommendations
1. **Re-engagement notifications** for users inactive >48 hours
2. **Fast-track credit offers** to users showing activity spikes
3. **In-app support** during credit application for users with high cancellation ratios

## Tech Stack
- Python (Pandas, NumPy, Scikit-learn, LightGBM, SHAP)
- SQL-style funnel analysis
- Matplotlib for visualization

## Files in This Repository
| File | Description |
| :--- | :--- |
| `fintech_funnel_analysis.ipynb` | Complete analysis notebook |
| `engineered_features.csv` | 15+ behavioral features for 5,000 users |
| `user_events.csv` | Raw synthetic event logs |
| `shap_importance_bars.png` | Feature importance visualization |

## How to Run
1. Open `fintech_funnel_analysis.ipynb` in Google Colab or Jupyter
2. Run all cells sequentially
3. The notebook will generate features, train the model, and produce SHAP analysis

## Author
**Ansh Chordiya** 

- [LinkedIn](www.linkedin.com/in/anshchordiya)
- [GitHub](https://github.com/anshchordiya)
