# Parkinson's Detection from Hand-drawn Spiral & Wave

A machine learning project that looks at a hand-drawn **spiral** or **wave** image and estimates whether it shows signs of Parkinson's disease (healthy vs. parkinson).

> Educational demo only. It is not a medical diagnosis tool.

## Team

| # | Name | Student ID |
|---|------|------------|
| 1 | Nazmul Hasan Jihan | _add ID_ |
| 2 | _teammate name_ | _add ID_ |
| 3 | _teammate name_ | _add ID_ |
| 4 | _teammate name_ | _add ID_ |

Course: _add course code_ | Instructor: _add professor name_

---

## Update 1 (20 October 2026)
- Project setup (repository, `.gitignore`, package list).
- Image preprocessing and feature extraction (`common.py`).
- Dataset description and project plan.

## Update 2

**Date:** _add date_

### What is included in Update 2
- Dataset added (`data.zip`, unzipped automatically into `data/` when the code runs).
- `train.py`: trains and compares 4 models separately for spiral and wave: SVM (RBF), Logistic Regression, Random Forest, Gradient Boosting.
- Each model is checked with 5-fold cross-validation, test accuracy, F1, AUC, and a stricter **subject-wise** accuracy (images from the same person are never split between train and test).
- The best model is chosen by cross-validation (not by the test set) and saved.
- Results are saved in the `outputs/` folder: `results.csv`, `comparison.png`, `confusion_spiral.png`, `confusion_wave.png`, `samples.png`.

### Who added which file

| Member | File(s) added in Update 2 | What it is |
|--------|---------------------------|------------|
| Nazmul Hasan Jihan | `README.md`, `requirements.txt` | Updated overview and package list |
| _Member 2 name_ | `train.py` | Model training and evaluation code |
| _Member 3 name_ | `data.zip` | Spiral and wave drawing images |
| _Member 4 name_ | `project_plan.md`, `outputs/` | Updated plan, and the result files created by running `train.py` |

### How to run
```
pip install -r requirements.txt
python train.py
```

### Results
_Paste the table from `outputs/results.csv` here after running `train.py`._

### Next steps (Update 3)
- Build the Streamlit web app (`app.py`) for prediction and for showing the results.
