
# 🏆 WIN THE BALL! SCORE GOALS AND WIN THE GAME!

Welcome to **WIN THE BALL!**, a Python project designed to analyze and compare detailed player statistics from top football (soccer) teams. This project allows you to explore player performance, expectations, and progression across matches, empowering you to uncover insights and win the game — both on the pitch and with your data!

---

## 📂 Project Overview

This project loads, processes, and analyzes player performance data from multiple football clubs (including Arsenal, Aston Villa, Bournemouth, Brighton, Chelsea, Fulham, Liverpool, Manchester City, Nottingham Forest, and Tottenham). It uses Python and pandas to handle `.xlsx` data files, preparing them for deeper analysis or visualization.

---

## 📊 Data Description

Each dataset includes the following sections:

### **Player Information**

* **Player**: Name
* **Nation**: Country of origin
* **Pos**: Position (e.g., FW, MF, DF, GK)
* **Age**: Player age (formatted as years-days)

### **Playing Time**

* **MP**: Matches played
* **Starts**: Number of games started
* **Min**: Minutes played
* **90s**: Number of full 90-minute games equivalent

### **Performance Metrics**

* **Gls**: Goals scored
* **Ast**: Assists made
* **G+A**: Goals + assists
* **G-PK**: Goals without penalty kicks
* **PK**: Penalty kick goals
* **PKatt**: Penalty kicks attempted
* **Crd-Y**: Yellow cards
* **Crd-R**: Red cards

### **Expected Metrics**

* **xG**: Expected goals
* **npxG**: Non-penalty expected goals
* **xAG**: Expected assisted goals
* **npxG + xAG**: Combined non-penalty and expected assisted goals

### **Progression Metrics**

* **prgC**: Progressive carries
* **prgP**: Progressive passes
* **prgR**: Progressive passes received

### **Per 90 Minutes (Per90) Stats**

All core metrics are also available normalized per 90 minutes, including:

* **Gls**, **Ast**, **G+A**, **G-PK**, **xG**, **npxG**, **xAG**, **npxG + xAG**

---

## 📦 Data Files

The project includes Excel files for each team:

* Arsenal.xlsx
* Aston\_Villa.xlsx
* Bournemouth.xlsx
* Brighton.xlsx
* Chelsea.xlsx
* Fulham.xlsx
* Liverpool.xlsx
* Manchester\_City.xlsx
* Nottingham.xlsx
* Tottenham.xlsx

Each file contains a detailed table of player stats.

---

## ⚙️ Setup Instructions

1️⃣ **Clone the repository**

```bash
git clone https://github.com/AmbroseJunior/premierLeagueData.git
cd premierLeagueData
```

2️⃣ **Install required packages**

```bash
pip install pandas openpyxl
```

3️⃣ **Download the data files**
Ensure all `.xlsx` files are placed in the project directory.

---

## 🏃 Running the Code

You can load and process a team's data using:

```python
import pandas as pd

# Example: Load Arsenal data
team1 = pd.read_excel('Arsenal.xlsx', decimal='.', index_col=0, header=1)
team1['Team'] = 'Arsenal'

# Display first few rows
print(team1.head())
```

Repeat for other teams by replacing the filename and team name.

---

## 🔍 What You Can Do

✅ Compare player performance across teams
✅ Analyze expected vs. actual performance
✅ Investigate progressive play contributions
✅ Normalize stats per 90 minutes for fair comparison
✅ Prepare custom visualizations (using pandas, matplotlib, seaborn, etc.)

---

## 🚀 Open In Colab

For a quick start, run this project in Google Colab:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

---

## 💡 Project Highlights

* 🏅 Combines raw match stats with advanced metrics
* 🔄 Easy data loading and merging across teams
* 📈 Ready for advanced analytics, ML, or dashboarding
* ⚽ Perfect for sports analysts, data scientists, or football fans

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## 🙌 Contributions

Feel free to open issues, submit pull requests, or suggest improvements!

