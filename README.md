# ML Model Training Hackathon Materials

This folder contains the teaching notes, presenter script, challenge brief, and a ready-to-run Jupyter notebook with three examples.

## Files

- `01_What_You_Should_Teach.md` — workshop concepts and definitions.
- `02_Live_Demonstration_Script.md` — step-by-step presenter notes.
- `03_Hackathon_Problem_Statement.md` — challenge brief, deliverables, rules, rubric, and schedule.
- `ML_Model_Training_Three_Examples.ipynb` — runnable notebook with Iris classification, Titanic survival classification, and Wine Quality regression.
- `README.md` — this guide.

## Recommended setup

**Easiest:** Google Colab  
1. Open https://colab.research.google.com/
2. Upload `ML_Model_Training_Three_Examples.ipynb`.
3. Run cells from top to bottom.
4. Accept the package-install cell if prompted.

**Local Jupyter:** Use Python 3.10+ and run the notebook with JupyterLab or Notebook. The first cell installs the required libraries.

## Dataset sources

- Iris CSV: public CSV hosted in the `mwaskom/seaborn-data` GitHub repository.
- Titanic CSV: public CSV hosted in the same repository.
- Wine Quality red wine CSV: UCI Machine Learning Repository.

Internet access is required to fetch the datasets. Dataset availability and third-party URLs can change; test the notebook before the workshop.

## Important teaching note

The notebook uses a single train/test split to keep the demo understandable. For a real competition or production model, use cross-validation where appropriate, keep a final test set untouched, check data leakage, and choose metrics based on the actual problem.

## Suggested workshop flow

1. Teach core concepts using `01_What_You_Should_Teach.md`.
2. Run the Iris example live using `02_Live_Demonstration_Script.md`.
3. Briefly compare the Titanic and Wine Quality examples.
4. Share `03_Hackathon_Problem_Statement.md` with teams.
5. Ask teams to submit their notebook, README, evaluation, and demo.
