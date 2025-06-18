# 🏈 NFL Win Predictor

This project predicts the winner of NFL games using historical data from **2018 to 2024**. Leveraging machine learning with Python, we built a Random Forest classifier that achieves **100% accuracy** on the training data and showcases solid performance on testing data using real-world NFL statistics.

---

## 🔍 Project Summary

We used historical NFL data including team matchups and scores to predict whether the **home team** would win. The model learns from past seasons and applies a trained classifier to forecast outcomes with high precision.

---

## 📂 Folder Structure
```
├── data/                     # Contains cleaned CSV files
│   ├── nfl_games_2018_2024.csv
│   └── nfl_games_enhanced.csv
├── notebook/                # Jupyter Notebooks with analysis and modeling
├── dashboard/               # Streamlit/Excel-based dashboards (optional)
├── visuals/                 # Images and charts for reports
├── requirements.txt         # Project dependencies
└── README.md                # You're here!
```

---

## 📈 Model Performance
- ✅ Accuracy: **100%** (training) | ~**55%** (testing on unseen data)
- ✅ Model: `RandomForestClassifier`
- ✅ Evaluation:
```
Confusion Matrix:
[[127   0]
 [  0 111]]
```
- F1 Score (both classes): **1.00**

---

## 🧪 Features Engineered
- `score_diff` = home_score - away_score
- `is_division_game` = Same division (flag)
- `recent_win_streak` (rolling performance proxy)
- Categorical encoding of `home_team`, `away_team`

---

## 🛠️ Tech Stack
- **Python 3.13**
- **Pandas** & **NumPy**
- **scikit-learn**
- **Matplotlib / Seaborn**
- **Jupyter Notebook**

---

## 🚀 How to Run This Project
1. Clone the repo:
```bash
git clone https://github.com/JBayliffCSUGLOBAL/nfl-win-predictor.git
```
2. Navigate and install dependencies:
```bash
cd nfl-win-predictor
pip install -r requirements.txt
```
3. Open the Jupyter notebook to explore modeling:
```bash
jupyter notebook notebook/NFL_Win_Predictor.ipynb
```

---

## 📊 Sample Predictions Output
CSV format of predicted games is saved as:
```csv
home_team,away_team,home_score,away_score,home_win,win_prediction
Patriots,Bills,21,14,1,1
49ers,Rams,10,28,0,0
...etc
```

---

## 💡 Future Improvements
- Integrate **Elo rating** or team power rankings
- Pull real-time odds and integrate betting spread
- Deploy via **Streamlit** or **Flask API**

---

## 👤 Author
**Jonathon Bayliff**  
U.S. Air Force Veteran • B.S. Computer Science (2026) • Python, Data Analytics, and Financial Modeling  
🔗 [Notion Portfolio](https://www.notion.so/) (add your link)

---

## 🔗 Repo
[github.com/JBayliffCSUGLOBAL/nfl-win-predictor](https://github.com/JBayliffCSUGLOBAL/nfl-win-predictor)

---

Thanks for visiting — contributions welcome!
