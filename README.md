# 🌌 Yuri Night: Asteroid Classification Model

🎉 A machine learning project to honor space exploration and planetary defense.

---

## 🛰️ Classification Overview

This repository contains an ML pipeline for classifying asteroids into:

- 🪐 **NEO (0)** – Near-Earth Objects  
- ☄️ **PHA (1)** – Potentially Hazardous Asteroids  
- 🌍 **NHA (2)** – Non-Hazardous Asteroids  

> Developed to celebrate [**Yuri’s Night**](https://yurisnight.net/) — the "World Space Party" 🌍🚀

---

## 🧠 What This Project Does

✅ Classifies asteroids using orbital and photometric data  
✅ Uses ML models like **KNN**, **SVM**, **Random Forest**, and **XGBoost**  
✅ Tackles class imbalance using **SMOTE**  
✅ Adds meaningful features like **MOID to SMA Ratio**  
✅ Visualizes patterns and skewness in the data

---

## 📊 Dataset Overview

Asteroid data includes:
- `H` – Absolute Magnitude  
- `a` – Semi-Major Axis  
- `q` – Perihelion Distance  
- `moid` – Earth MOID  
- `diameter`, `albedo`, `e`, `i`, etc.

Classification logic:
- **NEO:** `q` < 1.3 AU  
- **PHA:** `moid` ≤ 0.05 AU **and** `H` ≤ 22.0  
- **NHA:** All others

📁 Dataset Source: [NASA CNEOS NEO Dataset](https://cneos.jpl.nasa.gov/)

---

## 🤖 ML Models Used

- [K-Nearest Neighbors](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)  
- [Support Vector Machine](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)  
- [Random Forest](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)  
- [XGBoost Classifier](https://xgboost.readthedocs.io/en/stable/)

---

## ⚖️ Handling Class Imbalance

Initial class distribution was skewed.  
Applied **SMOTE** to balance class ratios manually to:

- 🪐 **NHA (2):** 30%  
- ☄️ **PHA (1):** 10%  
- 🌍 **NEO (0):** 10%

🔗 Learn about [SMOTE](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html)

---

## 📈 Visualizations

- 📊 Heatmaps (Asteroid type vs Year)  
- 📉 Histograms for skewness  
- 📌 Correlation matrices  
- 📊 Class bar plots

Built with [Seaborn](https://seaborn.pydata.org/) and [Matplotlib](https://matplotlib.org/)

---

## 📂 Project Structure
├── data/ ├── notebooks/ ├── src/ ├── visualizations/ └── README.md


---

## 🚀 Run Locally

```bash
# Clone the repo
git clone https://github.com/yourusername/yuri-night-asteroid-classifier.git

# Install dependencies
pip install -r requirements.txt

# Open Jupyter or run in Colab


---

Let me know if you want this saved in a `.md` file — or if you want dark/light mode badge support too.
