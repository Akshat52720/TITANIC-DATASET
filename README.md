# TITANIC-DATASET

# Titanic Exploratory Data Analysis (EDA)

This project explores the Titanic dataset to uncover patterns related to passenger survival. It combines data from `train.csv`, `test.csv`, and `gender_submission.csv`, performs feature engineering, and visualizes key relationships.

## Dataset Overview

- `train.csv`: Passenger features + survival labels
- `test.csv`: Passenger features (no survival labels)
- `gender_submission.csv`: Predicted survival for test set

## Objectives

- Clean and merge datasets
- Engineer meaningful features
- Visualize survival patterns
- Summarize key insights

## Tools & Libraries

- Python (pandas, numpy)
- Visualization: seaborn, matplotlib
- PDF Reporting
- Notebook: Jupyter / VS Code

---

## EDA Highlights

### Basic Exploration
- `.info()`, `.describe()`, `.value_counts()` used to inspect structure and distributions
- Missing values handled for `Age`, `Fare`, and `Embarked`

### Feature Engineering
- `FamilySize = SibSp + Parch + 1`
- `IsAlone = 1 if FamilySize == 1 else 0`
- `Title` extracted from `Name` and grouped

### Visualizations
- `pairplot` to explore relationships between features
- `heatmap` to show correlations
- Histograms, boxplots, scatterplots for detailed analysis

### Key Findings

| Feature      | Insight |
|--------------|--------|
| Gender       | Females had higher survival rates |
| Class        | First-class passengers more likely to survive |
| Fare         | Higher fare correlated with survival |
| IsAlone      | Alone passengers had lower survival odds |
| Title        | Social titles revealed survival patterns |

 ## Final Summary of Findings
 - Survival is strongly influenced by Fare, Pclass, and Gender.
 - Passengers traveling alone had lower survival rates.
 - Titles (like Mrs, Miss) may reflect social status and survival likelihood.
 - Higher Fare often indicates better class and higher survival.
 - Age is not a strong predictor alone but interacts with other features
