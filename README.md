# Kaggle Playground

Personal workspace for [Kaggle Playground Series](https://www.kaggle.com/competitions?hostSegmentIdFilter=8) competitions.

## Structure

```
playground_series/
  s5_12_Diabetes_Prediction_Challenge/   # Season 5, Episode 12
    eda/              # exploratory data analysis notebooks
    input             # competition datasets (symlink)
    ideas.md          # brainstorming & algorithm notes
    *.ipynb           # solution notebooks
    submission.csv    # latest submission
```

Each competition lives under `playground_series/`.

## Setup

```bash
uv sync          # install dependencies from pyproject.toml
```

### Adding Kaggle dataset paths to the venv

Create a `.pth` file in the venv's site-packages to make dataset paths available by default:

```bash
echo "/kaggle/input/your-dataset-name/" > .venv/lib/python3.13/site-packages/_kaggle.pth
```

## Key Dependencies

| Package | Purpose |
|---------|---------|
| xgboost | gradient boosting |
| scikit-learn | ML utilities & models |
| polars | fast dataframes |
| optuna | hyperparameter tuning |
| matplotlib / seaborn | plotting |

See [pyproject.toml](pyproject.toml) for the full list.
