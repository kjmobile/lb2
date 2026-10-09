# BA 320 Labs, 2026

Python labs for BA 320 (Introduction to Management Information Systems), Embry-Riddle Aeronautical University.
Each notebook follows the class slides and uses airline examples. Open one in Colab with its badge.

| # | Notebook | Open |
|---|---|---|
| 0 | Colab intro: SQL from Python, then one line fitted two ways | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/0_colab_intro.ipynb) |
| 1 | From a straight line to a curve, and a better input: airfares | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/1_LM_Linear_to_Polynomial_Airfares.ipynb) |
| 2 | Multiple regression and one-hot encoding: does the leading airline change fares? | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/2_LM_Multiple_Regression_one_hot_encoding_Airfares.ipynb) |
| A 0–2 | **Assignment (0-2):** simple and multiple regression for flight delays, with the weather as a category. Do it after notebooks 0–2 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/0-2_assignment.ipynb) |
| 3 | Feature engineering and regularization: polynomial features, overfitting, Lasso and Ridge | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/3_LM_Feature_engineering_and_regularization_Airfares.ipynb) |

In every notebook, look for **Your turn**: write the key modeling lines yourself, then open *Show answer* to check.

## Data

| File | What it is |
|---|---|
| `data/sabre_routes_2019.csv` | The 200 busiest U.S. domestic markets in 2019: distance, average fare, low-cost share, concentration, leading airline. Summarized from Sabre Market Intelligence (licensed to Embry-Riddle) for teaching. |

The class SQL database (`airline_db`, `hr`) holds sample data only.
