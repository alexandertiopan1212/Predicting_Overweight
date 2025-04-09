
# 🧠 Predicting Individual Weight using Support Vector Regression (SVR) from Scratch

Welcome to the **Predicting_Overweight** project! This repository showcases how we can leverage Support Vector Regression (SVR) — built entirely from scratch — to predict an individual’s weight based on lifestyle and physiological factors from an obesity dataset.

## 📌 Motivation

This project was inspired by a personal journey — from being 130 kg to becoming fit. The transformation sparked a deep curiosity: _can we mathematically predict someone's weight based on daily habits?_ The answer: YES, and here’s how.

---

## 🗂 Dataset Overview

Dataset: `ObesityDataSet_raw_and_data_sinthetic.csv`  
Entries: `2111` individuals

**Features include:**
- 🎂 Age, 👤 Gender, 📏 Height, ⚖️ Weight
- 🍔 High calorie food consumption (FAVC)
- 🥦 Vegetable consumption frequency (FCVC)
- 🥗 Meal frequency (NCP), 🍩 Snacking habits (CAEC)
- 🚬 Smoking habits, 🚰 Water intake (CH2O)
- 🔥 Physical activity (FAF), 📱 Tech usage (TUE)
- 🍻 Alcohol use (CALC), 🚗 Transportation mode (MTRANS)
- 📊 Obesity classification by WHO

---

## 📊 Exploratory Data Analysis

- Males generally weigh more than females.
- People with a family history of overweight or who consume high-calorie food frequently tend to weigh more.
- Public transport users showed higher average weights compared to walkers or bikers.
- Weak correlations found between weight and screen time or hydration.

---

## 🧮 Modeling: Support Vector Regression (from scratch)

No Scikit-learn magic here! Everything is built from scratch using:
- `NumPy`
- `cvxopt` for quadratic programming (solving SVR dual form)
- Custom `Gaussian Kernel` function
- `Min-Max Scaling` for normalization

### Hyperparameters
```python
c = 1.0         # Regularization
gamma = 1.0     # Gaussian kernel parameter
epsilon = 1.2   # Insensitive margin
```

---

## 🚀 Results

📈 R-squared: `0.6995`  
📉 Mean Squared Error: `211.94`

_Interpretation:_  
> The model explains ~70% of the variance in weight. Not bad for a handcrafted SVR model with non-linear kernel!

---

## 📍 Why This Project Matters

Predictive models like this can be a game-changer for:
- Personalized health monitoring
- Pre-emptive intervention against obesity
- Public health analytics

And it proves one thing: **Math can help you lose weight** (at least on paper 😉)

---

## 📂 Files
- `main.ipynb` – Full implementation, EDA + model training
- `ObesityDataSet_raw_and_data_sinthetic.csv` – The dataset
- `README.md` – You’re reading it 😎

---

## 🙌 Acknowledgements

Thanks to the creators of the dataset and the open-source community that makes machine learning accessible to all. This project is dedicated to those fighting their own health battles — you got this! 💪

---

Made with ❤️ by [alexandertiopan1212](https://github.com/alexandertiopan1212)

