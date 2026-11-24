# 📊 Cognifyz ML Internship

Machine learning tasks completed during my internship at **Cognifyz Technologies**, on a real restaurant dataset (Zomato-style: ratings, cuisines, locations, votes).

![Python](https://img.shields.io/badge/Python-3.13-3776AB?style=for-the-badge&logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.7-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

## 📈 Results

### Task 1 — Restaurant Ratings Prediction (regression)

| Model | RMSE | R² |
|:---|:---:|:---:|
| Linear Regression | 0.47 | 0.29 |
| Decision Tree | 0.37 | 0.55 |
| **Random Forest** | **0.34** | **0.63** |

Random Forest wins clearly — restaurant ratings depend on non-linear combinations of price, votes and location, which linear regression can't capture.

### Task 3 — Cuisine Classification (9 cuisines)

| Model | Accuracy | F1 |
|:---|:---:|:---:|
| Logistic Regression | 43.5% | 0.30 |
| **Random Forest** | **49.2%** | **0.42** |

Best class: **North Indian (F1 0.65)** — the most common cuisine in the data (599 test samples). Rare cuisines like Chinese (F1 0.07) are hard because the data is heavily imbalanced — an honest limitation, not a modelling failure.

### Task 4 — Location Analysis (exploratory)

- 🗺️ Mapped every restaurant with valid coordinates (latitude/longitude scatter plot)
- 🏙️ Ranked cities by restaurant count and by average rating (minimum 20 restaurants per city, so tiny samples don't skew the ranking)
- 🍜 Found the most common primary cuisine in each of the top 5 cities

## 📁 Tasks

| Notebook | What it does |
|:---|:---|
| `Task_1_Restaurant_Ratings.ipynb` | Predicts aggregate ratings — Linear Regression vs Decision Tree vs Random Forest |
| `Task_3_Cuisine_Classification.ipynb` | Classifies a restaurant's primary cuisine — Logistic Regression vs Random Forest |
| `Task_4_Location_Analysis.ipynb` | Geographic analysis — city rankings, rating maps, cuisine by city |
| `Dataset.csv` | Restaurant data used across all tasks |

## 🛠️ Tech Stack

Python · pandas · scikit-learn · matplotlib · Jupyter Notebook

## 🚀 Run it

```
git clone https://github.com/viju03-tech/Cognifyz-ML-Internship.git
cd Cognifyz-ML-Internship
pip install pandas scikit-learn matplotlib jupyter
jupyter notebook
```

Then open any `Task_*.ipynb` and run all cells.

## 👩‍💻 Author

**Viju B** — B.E. CSE, Sathyabama Institute of Science and Technology · [GitHub](https://github.com/viju03-tech) · [LinkedIn](https://www.linkedin.com/in/viju-b-4499823b4)
