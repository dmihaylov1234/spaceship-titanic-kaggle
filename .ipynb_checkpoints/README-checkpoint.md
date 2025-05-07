# ***Spaceship Titanic - Final Term Project for LING 539***

This project is based on an NLP modeling Kaggle challenge, [Spaceship Titanic Competition](https://www.kaggle.com/competitions/spaceship-titanic).

The purpose is to predict whether passengers were transported to an alternate dimension during the accident.  
This is framed as a **binary classification problem** using structured passenger data.

## Dataset

- Source: [Spaceship Titanic Kaggle Competition](https://www.kaggle.com/competitions/spaceship-titanic)
- Files: `train.csv` and `test.csv` provided by Kaggle

## Modeling Approach

- Preprocessing will include:
  - Handling missing values
  - Feature engineering (extracting **Deck**, **Cabin Number**, and **Side** from the `Cabin` column)
  - Encoding categorical features

- Models to be used:
  - **Random Forest** with hyperparameter tuning (`GridSearchCV`)
  - **XGBoost** classifier

- Evaluation metrics to be used:
  - **Accuracy**
  - **F1-Score**
  - Classification reports

## Results

| Model         | Accuracy | F1-Score |
|---------------|----------|----------|
| Random Forest | *0.80*   | *0.80*   |
| XGBoost       | *0.81*   | *0.81*   |


## Setup Instructions

### Option 1: Using pip

```bash
pip install -r requirements.txt
```

### Option 2: Using Conda
```bash
conda env create -f environment.yml
conda activate spaceship-titanic-env
```