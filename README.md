# Heart Disease Prediction

A machine learning project that predicts the presence of heart disease from patient medical data.

## Dataset
A messy ("dirty") heart disease dataset with 307 rows and 14 features (age, gender, chest pain type, blood pressure, cholesterol, max heart rate, and more). The target is `heart_disease_target` (1 = disease, 0 = no disease).

## Data Cleaning
The raw data had many issues that I fixed:
- Missing values and `?` placeholders
- Text mixed with numbers (e.g. `"54 years"`)
- Impossible values (negative cholesterol, age 300)
- Inconsistent gender labels (`M`, `F`, `1`, `unknown`)
- Decimal commas in `st_depression`

## Workflow
1. Load and inspect the data
2. Clean the data
3. Exploratory data analysis (correlations and visualizations)
4. Train a Random Forest classifier (80% train / 20% test)
5. Evaluate with accuracy, classification report and confusion matrix

## Results
| Model | Accuracy | Precision | Recall | F1-score |
|-------|----------|-----------|--------|----------|
| Random Forest | 0.80 | 0.79 | 0.79 | 0.79 |

## Project Structure
```
heart-disease-prediction/
├── data/
│   └── dirty_heart_disease_renamed.csv
├── notebooks/
│   └── heartdisease_clean.ipynb
├── README.md
└── requirements.txt
```

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook

## How to Run
1. Install the libraries: `pip install -r requirements.txt`
2. Open `notebooks/heartdisease_clean.ipynb` in Jupyter
3. Run all cells

## Author
Anas Mohamed - Data Science learner (IBM Data Science Professional Certificate)
