# OTTO E-Commerce Recommender System Challenge

![OTTO E-Commerce Recommender System Challenge Logo]([/mnt/data/image.png](https://storage.googleapis.com/kaggle-organizations/3827/thumbnail.png))

## Dataset Description

Welcome to the OTTO E-Commerce Recommender System Challenge! The objective of this competition is to develop a multi-objective recommender system that can accurately predict e-commerce activities such as clicks, cart additions, and orders based on previous user session events.

### Training Data

The training dataset (`train.jsonl`) provides comprehensive e-commerce session information. It includes:

- `session`: Unique identifier for the user session.
- `events`: A time-ordered sequence of events within the session, which includes:
  - `aid`: Article ID (product code) associated with the event.
  - `ts`: Unix timestamp when the event occurred.
  - `type`: Type of event (e.g., product click, cart addition, order).

### Test Data

The test dataset (`test.jsonl`) consists of truncated session data. The challenge is to predict the `aid` values for each session type that occur after the last event timestamp (`ts`) in the test session. Essentially, you're tasked with forecasting future e-commerce activities based on incomplete sessions.

### Objective

Your model should predict up to 20 future `aid` values for each session type (clicks, cart additions, orders) following the point of truncation in the test data.

### Files

- `train.jsonl` - Full session training data.
- `test.jsonl` - Truncated session test data, where the goal is to predict subsequent aids.
- `sample_submission.csv` - An example submission file in the correct format.

For additional information and background on this challenge, please refer to the published OTTO Recommender Systems Dataset on GitHub.

Good luck to all participants! Your innovative solutions will contribute to advancing e-commerce recommender systems.
