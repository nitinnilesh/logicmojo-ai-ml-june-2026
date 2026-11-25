# Hackathon Rules

## Team and time

- Teams contain 2–3 participants.
- Problem understanding: 20 minutes.
- Model development: 2 hours.
- Final submission must be received before the announced deadline.

## Allowed

- Classical machine-learning techniques covered in the course.
- Scikit-learn and XGBoost.
- Ensembles of your own trained classical models.
- Documentation and course materials.
- Feature engineering derived only from the provided features.

## Not allowed

- Neural networks or deep-learning frameworks for modelling.
- AutoML systems that search and build the complete solution automatically.
- External labelled data.
- Looking up or reconstructing hidden labels from the original public dataset.
- Manual labelling of test rows.
- Training preprocessing or resampling on validation/test data.
- Sharing code or predictions across teams.

## Validation and reproducibility

- Use a stratified validation strategy.
- `session_id` is an identifier and cannot be a model feature.
- Fix random seeds.
- The final notebook must run from top to bottom.
- Record every serious experiment, including one that did not help.

## Submission

- Submit probabilities, not hard labels.
- Required columns: `session_id,purchase_probability`.
- File name: `TEAM_NAME_submission.csv`.
- Maximum three hidden-test submissions per team.
- Only the best valid submission counts.

## Ranking

1. Highest hidden-test Average Precision.
2. Highest hidden-test ROC-AUC if AP is tied.
3. Earlier valid submission if both metrics are equal to four decimal places.

A team qualifies by reaching hidden-test AP of at least `0.55`.

## Integrity

The purpose is to demonstrate modelling judgment. Any hidden-label lookup or test-set leakage results in disqualification.
