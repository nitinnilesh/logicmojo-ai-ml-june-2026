# Metric Guide

## Why not accuracy?

Most sessions do not result in a purchase. A model can achieve high accuracy by predicting “no purchase” while failing to identify valuable sessions.

## Average Precision

Average Precision (AP) evaluates how effectively the model ranks actual purchasers above non-purchasers across decision thresholds.

- `1.0` is perfect.
- A random ranking has expected AP close to the purchase prevalence.
- Submit continuous probabilities; rounded 0/1 labels destroy ranking information.

AP is the leaderboard metric and must not be used to choose a hard threshold.

## Business threshold

A deployed system needs a decision such as “offer assistance” or “do not offer assistance.” Select a validation threshold that maximizes recall while maintaining precision of at least 40%.

- Precision asks: among contacted sessions, how many purchased?
- Recall asks: among all purchasers, how many did we reach?

Report the chosen threshold, precision, recall, predicted contact rate, and business interpretation.

## Tie-breaker

ROC-AUC is used only when two teams have the same AP to four decimal places.
