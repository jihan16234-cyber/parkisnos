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

## Update 1

**Date:** 20 October 2026

### What is included in Update 1
- Project setup (repository, `.gitignore`, package list).
- Image preprocessing: grayscale, resize, then black-and-white (Otsu threshold) so the pen stroke is white on black.
- Feature extraction: HOG (shape / tremor pattern) plus simple stroke statistics (ink amount, stroke length, number of contours, spread).
- Dataset description and project plan.

Model training (`train.py`) and the web app (`app.py`) come in the next updates.

### Who added which file

| Member | File(s) added in Update 1 | What it is |
|--------|---------------------------|------------|
| Nazmul Hasan Jihan | `README.md`, `.gitignore`, `requirements.txt` | Project overview, repo setup, package list |
| _Member 2 name_ | `common.py` | Image preprocessing and feature extraction code |
| _Member 3 name_ | `data_description.md` | Description of the spiral / wave dataset |
| _Member 4 name_ | `project_plan.md` | Plan for Updates 1, 2, 3 and the final report |

### Project files in this update
| File | Purpose |
|------|---------|
| `README.md` | Project overview and Update 1 summary |
| `.gitignore` | Files Git should ignore |
| `requirements.txt` | Python packages needed |
| `common.py` | Preprocessing and feature extraction |
| `data_description.md` | Dataset description |
| `project_plan.md` | Project plan by update |

### How to install
```
pip install -r requirements.txt
```

### Next steps (Update 2)
- Train and compare models (SVM, Logistic Regression, Random Forest, Gradient Boosting) with `train.py`.
- Add the dataset and save the results.
