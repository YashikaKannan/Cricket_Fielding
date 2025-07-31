# 🏏 Cricket Fielding Performance Analysis

This project analyzes individual fielding contributions of players from a T20 match to assess their overall performance using a weighted scoring system.

## Objective

To calculate the **Performance Score (PS)** of each player based on their fielding actions — catches, throws, run outs, etc.

### Dataset Features
- Match No.
- Innings
- Team
- Player Name
- Ballcount
- Position
- Short Description
- Pick (Clean Pick, Drop Catch, Catch, etc.)
- Throw (Run Out, Good Throw, Missed Run Out, etc.)
- Direct Hit
- Runs (Saved or Conceded)
- Overcount
- Venue

### 🧮 Performance Score Formula
PS = (CP×1) + (GT×2) + (C×10) + (DC×-10) + (ST×8) + (RO×10) + (MRO×-5) + (DH×3) + RS


Where:

- **CP**: Clean Picks  
- **GT**: Good Throws  
- **C**: Catches  
- **DC**: Dropped Catches  
- **ST**: Stumpings  
- **RO**: Run Outs  
- **MRO**: Missed Run Outs  
- **DH**: Direct Hits  
- **RS**: Runs Saved (+) / Conceded (-)

---

## 📊 Bar Chart Output

![Fielding Bar Chart](images/fielding_chart.png)

---

## 💻 Tech Used

- Python
- Pandas
- Matplotlib
- Google Colab / Jupyter Notebook

---

## 📁 How to Run

1. Clone this repo
2. Open `fielding_analysis.ipynb` in Google Colab or Jupyter
3. Run all cells to load data, compute metrics, and see visualization

---

## 📈 Output Example (from code)

| Player   | CP | GT | C | DC | ST | RO | MRO | DH | RS | Score |
|----------|----|----|---|----|----|----|-----|----|----|-------|
| Player 1 | 2  | 0  | 1 | 1  | 0  | 0  | 0   | 0  | -4 |  -2   |
| Player 2 | 2  | 1  | 1 | 0  | 0  | 1  | 1   | 1  |  2 |  24   |
| Player 3 | 1  | 1  | 0 | 0  | 0  | 0  | 0   | 0  |  1 |   4   |
