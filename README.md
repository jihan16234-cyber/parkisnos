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
- Project setup, image preprocessing and feature extraction (`common.py`), dataset description and project plan.

## Update 2
- Dataset added (`data.zip`) and `train.py` to train and compare 4 models (SVM, Logistic Regression, Random Forest, Gradient Boosting). Results saved in `outputs/`.

## Update 3

**Date:** _add date_

### What is included in Update 3
- `app.py`: a Streamlit web app with two tabs.
  - **Prediction:** choose spiral or wave, then upload an image, take a camera photo, or pick a sample from the dataset. The app shows the original image, the processed image, and the Parkinson's risk percentage.
  - **Project Results:** model comparison table, sample images, and confusion matrices from `outputs/`.
- If no saved model is found, the app trains the best model automatically on first start (takes 1-2 minutes).

### Who added which file

| Member | File(s) added in Update 3 | What it is |
|--------|---------------------------|------------|
| Nazmul Hasan Jihan | `README.md`, `requirements.txt` | Updated overview and package list (adds Streamlit) |
| _Member 2 name_ | `app.py` | The Streamlit web app |
| _Member 3 name_ | `project_plan.md` | Updated project plan |
| _Member 4 name_ | `screenshots/` | Screenshots of the running app (spiral and wave prediction, results tab) |

### How to run
```
pip install -r requirements.txt
python -m streamlit run app.py
```

### Next steps (Final)
- Add the final results, limitations and conclusion to the README.
