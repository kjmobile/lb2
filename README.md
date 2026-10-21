# BA 320 Labs, 2026

Python labs for BA 320 (Introduction to Management Information Systems), Embry-Riddle Aeronautical University.
Each notebook follows the class slides and uses airline examples. Open one in Colab with its badge.

Every lab comes in two versions:

- **`_simple`** (the badges below): the code that fits the model and produces the results. Figures are shown as pictures.
- **`_all`**: the same notebook plus the code that draws every figure. Open it when you want to make or change a chart.

| # | Notebook | Open |
|---|---|---|
| 0 | Colab intro: get flight delays with SQL, then one regression for two goals (statistical inference vs. machine-learning prediction) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/0_colab_intro_simple.ipynb) |
| 1 | From a straight line to a curve, and a better input: airfares | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/1_LM_Linear_to_Polynomial_Airfares_simple.ipynb) |
| 2 | Multiple regression and one-hot encoding: does the leading airline change fares? | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/2_LM_Multiple_Regression_one_hot_encoding_Airfares_simple.ipynb) |
| A 0–2 | **Assignment (0-2):** simple and multiple regression for flight delays, with the weather as a category. Do it after notebooks 0–2 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/0-2_assignment.ipynb) |
| 3 | Feature engineering and regularization: polynomial features, overfitting, Lasso and Ridge | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/3_LM_Feature_engineering_and_regularization_Airfares_simple.ipynb) |
| 4 | Logistic regression: is a booking a business or a leisure trip? Probabilities, odds, the 0.5 cut-off, accuracy against a baseline | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/4_Logistic_Regression_Business_or_Leisure_simple.ipynb) |
| 5 | Naive Bayes: no-shows in 20 practice bookings (Bayes' theorem, base rates, the naive shortcut), then late flights | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/5_Naive_Bayes_No_Shows_and_Late_Flights_simple.ipynb) |
| 6 | Decision tree: which flights will arrive late? Overfitting, pruning, information gain, feature importance | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/6_Decision_Tree_Late_Flights_simple.ipynb) |
| 7 | Validation set, k-fold cross-validation, grid search and random search | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/7_Cross_Validation_and_Grid_Search_Late_Flights_simple.ipynb) |
| 8 | Ensembles: random forest (bagging, OOB score), AdaBoost, gradient boosting | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/8_Ensemble_Random_Forest_and_Boosting_Late_Flights_simple.ipynb) |
| 9 | K-nearest neighbors: which markets do American, Delta or United lead? Distance, standardization, choosing k | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/9_KNN_Hub_Carrier_Markets_simple.ipynb) |
| 10 | K-means clustering: kinds of airline markets, the elbow method | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/10_KMeans_Clustering_Airline_Markets_simple.ipynb) |
| 11 | Principal component analysis: five market numbers on two axes, loadings, eigenvalues | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/11_PCA_Airline_Markets_simple.ipynb) |
| 12 | Support vector machine: a straight and a curved boundary, support vectors, the C setting | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/12_SVM_Hub_Carrier_Markets_simple.ipynb) |
| 13 | Neural networks with TensorFlow/Keras: the XOR problem, then a multilayer perceptron for late flights | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kjmobile/lb2/blob/main/13_Neural_Network_XOR_and_Late_Flights_simple.ipynb) |

In every notebook, look for **Your turn**: write the key modeling lines yourself, then open *Show answer* to check.

## Data

| File | What it is |
|---|---|
| `data/sabre_routes_2019.csv` | The 200 busiest U.S. domestic markets in 2019: distance, average fare, low-cost share, concentration, leading airline. Summarized from Sabre Market Intelligence (licensed to Embry-Riddle) for teaching. |
| `data/booking_lead_days.csv` | 983 air bookings from 2023, two columns only: days booked ahead and whether the trip was business (1) or leisure (0). From an Amadeus bookings sample (licensed to Embry-Riddle), for teaching. |
| `data/noshow_20.csv` | 20 made-up bookings for teaching Bayes' theorem (no-show, refundable fare, booked 60+ days out, checked bag). Not real airline statistics. |
| `data/flights_late_2024.csv` | 2,000 U.S. domestic flights from 2024, sampled at random: month, departure hour, distance, how late the incoming plane arrived, scheduled turn time, and whether the flight arrived 15+ minutes late. From the BTS on-time records (public data). |
| `data/img/` | The figures shown in the `_simple` notebooks, drawn by the `_all` notebooks. |

The class SQL database (`airline_db`, `hr`) holds sample data only.
