# cmu-mlip-model-testing-lab

## Quick setup
- Python 3.10+
- Install deps:
  ```bash
  pip install -r requirements.txt
  ```
- Login to W&B:
  ```bash
  wandb login
  ```

## What the notebook does (`lab4.ipynb`)
- Loads a tweet sentiment dataset.
- Runs a baseline model and a candidate model.
- Creates hypothesis-driven slices (hashtags, mentions, negation, emoji density, tweet length, URLs).
- Computes overall and slice metrics, then logs `df_long`, `slice_metrics`, `regression_metrics`, and `df_eval` to W&B.
- Visualizes slice performance in W&B to spot regressions.
- Stress-tests a weak slice with 10 LLM-generated tweets and compares model behavior.

## How to run
- Open `lab4.ipynb` and run cells top to bottom.
- Keep short notes in `saved_slice_notes` for each slice.
