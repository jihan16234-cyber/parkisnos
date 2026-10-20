# Parkinson's Detection from Hand-drawn Spiral & Wave

A machine learning project that looks at a hand-drawn **spiral** or **wave** image and estimates whether it shows signs of Parkinson's disease (healthy vs. parkinson). It includes a Streamlit web app to try it out.

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

## How it works
1. **Preprocess:** grayscale, resize (spiral 128x128, wave 256x128), then black-and-white (Otsu threshold) so the pen stroke is white on black.
2. **Features:** HOG (shape / tremor pattern) plus simple stroke statistics (ink amount, stroke length, number of contours, spread).
3. **Models:** SVM (RBF), Logistic Regression, Random Forest, Gradient Boosting, trained separately for spiral and wave.
4. **Evaluation:** 5-fold cross-validation, test accuracy, F1, AUC, and **subject-wise** accuracy (images from the same person are never split between train and test). The best model is chosen by cross-validation, not by the test set.
5. **App:** upload an image, take a camera photo, or pick a dataset sample, and see the Parkinson's risk percentage.

## Project files

| File | Purpose | Added in |
|------|---------|----------|
| `common.py` | Image preprocessing and feature extraction | Update 1 |
| `data_description.md` | Dataset description | Update 1 |
| `train.py` | Trains and evaluates the models, saves results in `outputs/` | Update 2 |
| `data.zip` | Spiral and wave drawing images | Update 2 |
| `app.py` | Streamlit web app | Update 3 |
| `requirements.txt` | Python packages needed | Update 1-3 |
| `project_plan.md` | Plan and status by update | Update 1-Final |

## How to run
```
pip install -r requirements.txt
python train.py
python -m streamlit run app.py
```

## Results
_Paste the table from `outputs/results.csv` here, and add the `comparison.png` and confusion matrix images._

| Dataset | Model | CV acc | Test acc | F1 | AUC | Subject-wise acc |
|---------|-------|--------|----------|----|-----|------------------|
| _spiral_ | _model_ | _value_ | _value_ | _value_ | _value_ | _value_ |
| _wave_ | _model_ | _value_ | _value_ | _value_ | _value_ | _value_ |

## Limitations
- The dataset is small, so results can change a lot with a different split.
- Drawings are taken on paper and photographed, so lighting and pen type can affect the result.
- This is a screening-style demo and cannot replace a doctor's diagnosis.

## Team contributions

| Member | Contribution |
|--------|--------------|
| Nazmul Hasan Jihan | _what you did_ |
| _Member 2 name_ | _what they did_ |
| _Member 3 name_ | _what they did_ |
| _Member 4 name_ | _what they did_ |

## Conclusion
_Write 2-3 lines about what worked best and what you would improve next._
