# FPL Player Analytics

This repository contains data analysis for Fantasy Premier League (FPL) player statistics. The project focuses on cleaning, transforming, and analyzing player data to help make informed decisions in FPL.  

---

## 📂 Project Structure

- `fpl_player_statistics.csv` — Original raw FPL player dataset.  
- `fpl_player_statistics_cleaned.csv` — Cleaned dataset after removing unnecessary columns and handling missing values.  
- `data_analysis.ipynb` — Jupyter Notebook containing Python data cleaning, transformations, and analysis.  
- `Dashboard 1.pdf` — Tableau dashboard visualizing key FPL metrics and player performance.  
- `README.md` — Project documentation.

---

## 🧹 Data Cleaning

The following steps were performed on the raw data:

1. Removed redundant or noisy columns, such as detailed statistics not relevant for general analysis.  
2. Handled missing values:
   - Blank `news` fields were replaced with "No News".  
   - Missing numeric values were imputed or left as 0 depending on context.  
3. Standardized column headers:
   - Converted underscores `_` to spaces.  
   - Capitalized the first letter of each word for readability.

---

## 📊 Analysis

Using Python, Excel, and Tableau:

- Created calculated metrics to help evaluate players, including:
  - **Points per Million** — Efficiency of player points relative to cost.  
  - **Attack Involvement** — Goals + assists contribution.  
  - **Points per Start** — Average points scored per match played.  
  - **ROI (Return on Investment)** — Value analysis based on points vs. cost.  
  - **Minutes per Point** — How often the player contributes points per minutes played.  
- Ranked players based on `Smart Player Selector` scores to identify top-performing players.  
- Filtered and sorted data to focus on top players efficiently.  

---

## 📈 Tableau Dashboard

An interactive Tableau dashboard was created to visualize:

- **Top Players by Total Points** — Bar chart showing leading scorers.  
- **Value vs Cost (ROI)** — Scatter plot analyzing cost efficiency.  
- **Efficiency (Minutes per Point)** — Relationship between points per start and total points.  
- **Points per Million by Club** — Treemap comparing club performance.  
- **Points per Million by Position** — Breakdown of player efficiency across positions (DEF, FWD, GKP, MID).  

The dashboard helps quickly identify high-value players and make data-driven FPL decisions.

---

## 💻 Tools Used

- **Python (Jupyter Notebook)** — For cleaning, processing, and analyzing the data.  
- **Excel** — For additional calculations, filtering, and creating helper columns.  
- **Tableau** — For creating interactive visualizations and dashboards.  

---

## 🔧 Usage

1. Clone the repository:  
```bash
git clone https://github.com/your-username/fpl-player-analytics.git
```

2. Open `data_analysis.ipynb` in Jupyter Notebook or VS Code.

3. Load the cleaned CSV file (`fpl_player_statistics_cleaned.csv`) for analysis:
```python
import pandas as pd

df = pd.read_csv('fpl_player_statistics_cleaned.csv')
```

4. Use the notebook or Excel to explore player statistics, calculate metrics, and sort/filter players.

5. View the Tableau dashboard (`Dashboard 1.pdf`) for visual insights, or open the Tableau workbook (`.twbx` file if included) to interact with live visualizations.

---

## 📈 Insights

* Identify top-performing players based on `Smart Player Selector` or custom metrics.
* Compare players efficiently based on cost, points, and contribution metrics.
* Filter by position, club, or other relevant statistics to shortlist FPL candidates.
* Use visual dashboards to spot trends and patterns in player performance.

---

## ⚡ Contribution

Feel free to fork this repository, add your own analysis, or contribute improvements.

---

## 📄 License

This project is open source under the MIT License.
