# 🧪 Basic Machine Learning — Sample Notebooks

Welcome to the **Basic Machine Learning** track for **AuraGen 2026**. These notebooks introduce the end-to-end ML workflow using familiar datasets and classical machine-learning algorithms.

## 📘 What's inside?

### 1. Iris Flower Classification
**Notebook:** [`01_Iris_Flower_Classification.ipynb`](./01_Iris_Flower_Classification.ipynb)

- Explore flower measurements and target labels
- Prepare training and testing data
- Scale features
- Train a Logistic Regression classifier
- Evaluate accuracy and inspect a confusion matrix

### 2. Titanic Survival Prediction
**Notebook:** [`02_Titanic_Survival_Classification.ipynb`](./02_Titanic_Survival_Classification.ipynb)

- Handle missing values
- Encode categorical features
- Build a classification model
- Evaluate predictions with classification metrics
- Predict survival for a new passenger

### 3. Wine Quality Prediction
**Notebook:** [`03_Wine_Quality_Regression.ipynb`](./03_Wine_Quality_Regression.ipynb)

- Explore numerical features
- Prepare data for training
- Train a regression model
- Evaluate predictions with regression metrics
- Understand how feature values relate to predicted quality

## 🖼️ Notebook overview

![Basic ML notebook examples](./Images/Simple.jpg)

## ⚙️ Requirements

- Python 3.10 or newer recommended
- Jupyter Notebook, JupyterLab, or Google Colab
- The notebook-specific libraries listed in each notebook's setup cells

Common packages include:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

Some notebooks may install or require additional packages. Follow the setup instructions inside each notebook.

## 🚀 How to run

### Option A — Google Colab
1. Open a notebook from this folder on GitHub.
2. Download it or upload it to [Google Colab](https://colab.research.google.com/).
3. Run the cells from top to bottom.

### Option B — Run locally
1. Clone or download this repository.
2. Open a terminal in the repository folder.
3. Install the required packages.
4. Start Jupyter:

```bash
jupyter notebook
```

5. Open a notebook and run the cells in order.

## 🎯 Suggested basic-track challenge

Choose a classification dataset, train **two classical ML algorithms**, and compare their results using the same train/test split and suitable metrics. Explain which model performs better and why. Include a confusion matrix when appropriate.

## 📊 What participants should submit

- A working notebook with clear comments
- A short explanation of the dataset and target
- Results from both algorithms
- A fair comparison using suitable evaluation metrics
- A brief conclusion describing limitations and possible improvements

## 💡 Learning outcome

By completing these examples, participants should understand the core ML workflow: **load data → explore → preprocess → split → train → evaluate → predict**.

---

Part of the **AuraGen 2026** machine-learning workshop. Learn the fundamentals, experiment responsibly, and explain your results clearly.
