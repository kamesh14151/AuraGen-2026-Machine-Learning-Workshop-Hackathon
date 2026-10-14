# Live Demonstration — What to Say While Coding

Use this as a presenter script while running `ML_Model_Training_Three_Examples.ipynb`.

## Opening (1–2 minutes)

“Today we’ll build machine-learning models from real datasets. We will not just import a model and make a prediction. We’ll follow the full workflow: understand the data, prepare it, train a model, evaluate it on unseen data, and make a prediction.”

## Step 1 — Install and import libraries

**Show:** The dependency installation and import cells.

**Say:** “Pandas helps us inspect tables. Scikit-learn gives us algorithms and evaluation tools. The datasets are small enough to run on a regular laptop or Google Colab; no GPU is required.”

**Ask:** “What do you think a model needs before it can learn?”

Expected answer: examples, input features, and—when supervised learning is used—known labels.

## Step 2 — Load and inspect the dataset

**Show:** `load_dataset` / `pd.read_csv`, `head()`, `shape`, `info()`, and missing-value counts.

**Say:** “Never start by training blindly. First inspect the dataset. We need to understand what one row represents, what each column means, and whether values are missing.”

**Ask:** “Which column is the answer we want the model to predict?”

## Step 3 — Separate features and target

**Show:** `X = ...` and `y = ...`.

**Say:** “`X` contains the inputs. `y` contains the correct answer. During training, the model tries to learn a relationship between them.”

For Iris: inputs are flower measurements; target is species.  
For Titanic: inputs are passenger details; target is survival.  
For Wine Quality: inputs are chemical measurements; target is a numeric quality score.

## Step 4 — Split the data

**Show:** `train_test_split(...)`.

**Say:** “We keep some examples out of training so we can test whether the model generalizes. If we test on the same rows used for training, the score can be misleading.”

For classification, explain `stratify=y`. For the wine regression example, do not use `stratify`.

## Step 5 — Preprocess and train

**Show:** The pipeline, preprocessing steps, model definition, and `.fit()` call.

**Say:** “Real data can contain missing values and categories. Our pipeline applies the required transformations and then trains the model. The transformations are fitted from training data, which helps avoid test-data leakage.”

Explain:
- Logistic Regression: a simple classification baseline.
- Random Forest: a collection of decision trees.
- Random Forest Regressor: predicts a number rather than a category.

## Step 6 — Evaluate

**Show:** Accuracy, classification report, confusion matrix, or regression metrics.

**Say:** “A metric is useful only if we understand what it measures. Accuracy is easy to explain, but precision, recall, and F1-score matter when classes are imbalanced. For numeric predictions, MAE tells us the average absolute prediction error.”

**Ask:** “If two models have similar accuracy, what else would you compare?”

Expected answers: recall, precision, F1-score, errors by class, interpretability, speed, and performance on additional validation data.

## Step 7 — Compare models

**Show:** Results from Logistic Regression and Random Forest for classification.

**Say:** “We are comparing models on the same split. One result does not prove a model is universally better. On small datasets, results can change with the split; cross-validation is a useful next step.”

## Step 8 — Make a new prediction

**Show:** The sample input and `model.predict(...)`.

**Say:** “Training is not the end. The model is useful when we can pass it new input and receive a prediction. In a real application, the input must use the same columns and preprocessing expected during training.”

## Step 9 — Save the model

**Show:** `joblib.dump(...)`.

**Say:** “Saving the pipeline preserves both preprocessing and the trained estimator. A deployment can load this file later, but only load model files you trust.”

## Close and transition to challenge

“You’ve now seen the complete workflow. Your task is to apply it to a new problem. Your goal is not just the highest score: show that your data preparation is correct, your evaluation is fair, and your solution can make a prediction on new input.”

## Suggested timing

| Activity | Time |
|---|---:|
| Fundamentals | 10–15 min |
| Iris demo | 10 min |
| Titanic demo | 10–15 min |
| Wine Quality demo | 10 min |
| Questions and challenge briefing | 5 min |

If the workshop slot is short, run Iris live and explain the other two examples, then let participants explore all three in the notebook afterward.
