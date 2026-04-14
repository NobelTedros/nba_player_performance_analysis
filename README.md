# 🏀 NBA Player Performance Analysis

Exploratory data analysis and linear regression on NBA player statistics from 2000–present.
Built to answer one question: **what actually separates elite scorers from everyone else?**

---

## Dataset

**NBA Players Stats** by Justinas Cirtautas — [Kaggle link](https://www.kaggle.com/datasets/justinas/nba-players-data)

The dataset contains season-level stats for every NBA player from 1996 to 2022, including
points, rebounds, assists, usage rate, true shooting %, net rating, and more.

---

## Tools Used

- **Python** — pandas, NumPy, SciPy, scikit-learn
- **Visualization** — Matplotlib, Seaborn
- **Statistics** — Pearson correlation, train/test split, StandardScaler, LinearRegression

---

## Key Findings

1. **Usage rate (usg_pct) is the strongest predictor of scoring** — Pearson r ≈ 0.80. Volume of touches matters more than efficiency.
2. **True Shooting % is weakly correlated with raw points** — High-efficiency role players take fewer shots by design, so TS% alone does not predict scoring output.
3. **Height and weight have near-zero correlation with points** — The modern NBA has fully decoupled physical size from scoring ability.
4. **A simple 4-feature linear regression achieves R² ≈ 0.65–0.70** — Usage, efficiency, assists, and net rating explain most of scoring variance. The remaining gap reflects shot selection and coaching decisions that box scores cannot capture.

---

## How to Run

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/nba-player-performance-analysis.git
cd nba-player-performance-analysis
```

### 2. Download the dataset
- Go to: https://www.kaggle.com/datasets/justinas/nba-players-data
- Click **Download** (free Kaggle account required)
- Unzip the file — you'll get `all_seasons.csv`
- Place `all_seasons.csv` in the **same folder as the notebook**

### 3. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter
```

### 4. Run the notebook
```bash
jupyter notebook nba_player_performance_analysis.ipynb
```
Then: **Kernel → Restart & Run All**

---

## Project Structure

```
nba-player-performance-analysis/
├── nba_player_performance_analysis.ipynb   # Main analysis notebook
├── README.md                               # This file
└── all_seasons.csv                         # Dataset (download from Kaggle — not included)
```

---

## Author

**Nobel Tedros** — Virginia Tech, B.S. Computational Modeling & Data Analytics  
[LinkedIn](https://www.linkedin.com/in/nobel-tedros-b08044262)
