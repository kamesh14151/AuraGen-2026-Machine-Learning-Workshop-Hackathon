# Hackathon Track: ML Model Training Challenge

## Theme
**Build, Train, Evaluate, Predict**

## Problem statement

Build a machine-learning solution for a provided dataset. Your team must investigate the data, prepare it correctly, train and compare models, evaluate performance on unseen data, and demonstrate a prediction.

The organizers may assign one of these problem types:
- **Classification:** Predict a category, such as a flower species or passenger survival.
- **Regression:** Predict a numeric value, such as a quality score.

## Objectives

1. Understand the dataset and define the target.
2. Identify useful features and inspect data quality.
3. Handle missing values and categorical features where applicable.
4. Split data into training and test sets.
5. Train at least two suitable algorithms.
6. Compare models with appropriate evaluation metrics.
7. Visualize results and explain errors.
8. Demonstrate at least one prediction on new input.
9. Explain limitations, assumptions, and potential bias.

## Required deliverables

- A runnable Jupyter Notebook (`.ipynb`).
- A short README describing the problem, dataset, features, target, and approach.
- Results from at least two models.
- At least one chart or confusion matrix (for regression, use a suitable actual-vs-predicted plot).
- A saved model file if time permits.
- A 3–5 minute team presentation or demo.

## Rules

- Use the dataset assigned by the organizers.
- Keep the test set separate from model fitting and tuning.
- Do not report training accuracy as the final performance.
- Do not use target information that would not be available at prediction time.
- Clearly state any external datasets, pretrained models, or extra tools used.
- Make sure another team member or judge can run the notebook from top to bottom.
- Explain the approach; a copied notebook without understanding will not receive full credit.

## Judging rubric — 100 points

| Criterion | Points | What judges look for |
|---|---:|---|
| Data understanding and preprocessing | 20 | Correct target, sensible cleaning, feature handling |
| Training methodology | 20 | Valid split, reproducible training, no obvious leakage |
| Model experimentation | 20 | At least two models and a meaningful comparison |
| Evaluation and visualization | 20 | Appropriate metrics and clear interpretation |
| Demo, explanation, and reproducibility | 20 | Working predictions, clear presentation, runnable notebook |

## Bonus opportunities

- Use cross-validation.
- Tune a hyperparameter and explain why.
- Address class imbalance appropriately.
- Build a small web interface for predictions.
- Explain fairness, privacy, or real-world deployment limitations.

## Suggested 75-minute schedule

- 10 minutes — Read the dataset and define the target.
- 15 minutes — Explore and preprocess.
- 20 minutes — Train at least two models.
- 15 minutes — Evaluate, compare, and visualize.
- 10 minutes — Prepare the demo and README.
- 5 minutes — Submit.

## Submission checklist

- [ ] Notebook runs from top to bottom.
- [ ] Features and target are clearly identified.
- [ ] Train/test split is documented.
- [ ] At least two models are compared.
- [ ] Evaluation metrics are appropriate.
- [ ] At least one visualization is included.
- [ ] Limitations are explained.
- [ ] Prediction demo works.
