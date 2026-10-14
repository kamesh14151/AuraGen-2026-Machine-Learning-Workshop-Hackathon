# ML Model Training Workshop — What You Should Teach

**Audience:** Beginner-level hackathon participants  
**Suggested duration:** 20–30 minutes of concepts, followed by live coding  
**Goal:** Help participants understand the end-to-end workflow for training and evaluating a machine-learning model.

## 1. What is Machine Learning?

Machine Learning (ML) is a way to build systems that learn patterns from examples and use those patterns to make predictions on new data.

**Example:** Instead of writing rules for every flower species, we provide flower measurements and their known species. An algorithm learns patterns from those examples.

## 2. Main types of machine learning

- **Supervised learning:** Data includes the correct answer (label). Examples: predicting a flower species or passenger survival.
- **Unsupervised learning:** Data has no target labels; the model looks for structure or groups.
- **Reinforcement learning:** An agent learns by taking actions and receiving rewards or penalties.

For this workshop, focus on **supervised learning**.

## 3. Important terms

| Term | Meaning | Example |
|---|---|---|
| Dataset | A collection of examples | Records about flowers |
| Row / sample | One example | One flower |
| Feature (`X`) | Input used to make a prediction | Petal length |
| Target / label (`y`) | What we want to predict | Flower species |
| Classification | Predict a category | Survived / did not survive |
| Regression | Predict a numeric value | Wine quality score |
| Training | Learning patterns from training examples | `model.fit(X_train, y_train)` |
| Inference | Predicting for new data | `model.predict(new_data)` |

## 4. The standard ML workflow

1. Define the problem and target.
2. Load the dataset.
3. Explore rows, columns, data types, missing values, and target distribution.
4. Separate features (`X`) and target (`y`).
5. Split the data into training and testing sets.
6. Preprocess the data.
7. Train a baseline model.
8. Evaluate on unseen test data.
9. Compare models or tune parameters.
10. Make predictions and save the model.

## 5. Train/test split

A common beginner-friendly split is 80% training data and 20% test data.

- The **training set** is used to fit the model.
- The **test set** is held back to estimate performance on unseen examples.
- Never use test data to fit preprocessing steps or tune model choices.

For classification, `stratify=y` can help preserve class proportions across the splits.

## 6. Preprocessing

Real datasets are often messy. Common steps include:

- Handling missing numeric values (for example, median imputation).
- Handling missing categorical values (for example, most-frequent imputation).
- Encoding text categories as numeric values.
- Scaling numeric features when an algorithm benefits from it.
- Checking duplicates, unusual values, and target imbalance.

Use a scikit-learn `Pipeline` and `ColumnTransformer` where possible. This keeps preprocessing and model training together and reduces data leakage.

## 7. Models in the notebook

- **Logistic Regression:** A useful baseline for classification. Despite its name, it is commonly used to predict categories.
- **Random Forest:** Combines many decision trees and can model nonlinear patterns.
- **Random Forest Regressor:** Predicts numeric values, such as wine quality scores.

No algorithm is best for every dataset. Compare results using the same split and appropriate metrics.

## 8. Evaluation metrics

### Classification
- **Accuracy:** Percentage of predictions that are correct.
- **Precision:** Of the examples predicted as a class, how many were correct?
- **Recall:** Of all real examples in a class, how many did the model identify?
- **F1-score:** Harmonic mean of precision and recall.
- **Confusion matrix:** Shows correct and incorrect predictions by class.

### Regression
- **MAE (Mean Absolute Error):** Average absolute difference between predictions and true values; lower is better.
- **RMSE (Root Mean Squared Error):** Penalizes large errors more heavily; lower is better.
- **R²:** Measures variance explained relative to a mean-baseline; closer to 1 is generally better, but interpret it in context.

## 9. Overfitting and data leakage

- **Overfitting:** A model performs very well on training examples but poorly on unseen examples.
- **Data leakage:** Information that would not be available at prediction time, or information from the test set, influences training.
- A very high score is not automatically proof of a strong real-world model.

## 10. Three examples used in the notebook

1. **Iris classification:** Predict flower species from four numeric measurements.
2. **Titanic survival classification:** Predict survival from passenger information, handling missing and categorical values.
3. **Wine quality regression:** Predict a numeric quality score from chemical measurements.

## 11. Questions to ask participants

1. What are the features and target in each example?
2. Why do we keep a test set separate?
3. Why can accuracy be misleading on imbalanced data?
4. What does the confusion matrix tell us?
5. Why is preprocessing included in a pipeline?
6. How does classification differ from regression?
7. What limitations might prevent a model from working well in the real world?

## 12. Instructor reminder

Run the notebook once before the session and ensure the room has internet access. The notebook downloads public datasets. If network access is unreliable, download the datasets in advance and update the URLs to local file paths.
