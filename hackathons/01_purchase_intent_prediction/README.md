# Purchase Intent Prediction Hackathon

Build a classical machine-learning model that estimates the probability that an e-commerce browsing session will end in a purchase.

## Format

- 20 minutes: understand the problem, data and metric
- 2 hours: develop and validate the solution
- 40 minutes: team presentations
- Team size: 2–3 participants

## Success Criteria

- Primary leaderboard metric: **Average Precision (AP)**
- Minimum qualifying hidden-test AP: **0.55**
- Tie-breaker: **ROC-AUC**
- Business task: maximize validation recall while maintaining precision of at least 40%

The leaderboard score is calculated directly from submitted probabilities. The hidden test labels remain with the instructor.

## Files

| File | Purpose |
| --- | --- |
| `purchase_intent_hackathon.ipynb` | Starter notebook with the problem workflow and TODOs |
| `train.csv` | Labelled sessions for model development |
| `test.csv` | Unlabelled sessions for final probability prediction |
| `sample_submission.csv` | Required submission structure |
| `RULES.md` | Permitted techniques, integrity rules and submission limits |
| `METRIC_GUIDE.md` | Average Precision and business-threshold guidance |
| `PRESENTATION_GUIDE.md` | Required structure for the team presentation |

## Getting Started

1. Download this folder or clone the repository.
2. Keep the notebook and CSV files in the same directory.
3. Open `purchase_intent_hackathon.ipynb` in Google Colab or Jupyter.
4. Read `RULES.md` and `METRIC_GUIDE.md` before modelling.
5. Use local validation to select the final approach.
6. Generate probabilities for every row in `test.csv`.

## Submission

Submit one CSV named `TEAM_NAME_submission.csv` with exactly these columns:

```text
session_id,purchase_probability
100101,0.8214
100102,0.1738
```

- Do not submit predicted class labels.
- Every test `session_id` must appear exactly once.
- Probabilities must be finite and between 0 and 1.
- Each team may make at most three hidden-test submissions.

The instructor will match `session_id` with the private labels, calculate AP and ROC-AUC, and update the leaderboard.

## Dataset

The challenge is derived from the UCI Online Shoppers Purchasing Intention dataset. The supplied split uses a fixed stratified partition so that training and hidden-test purchase rates remain comparable.
