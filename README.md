# 🎾 ATP 2025 Upset Match Analysis

**Course:** MESA 8411 – Programming for Data Science  
**Author:** Gaeul "Alice" Lee

---

## 📌 Project Overview

This project analyzes **upset matches** in the 2025 ATP Tour — matches where the lower-ranked player defeats the higher-ranked player. Upsets are among the most exciting moments in tennis, making tournaments feel unpredictable and competitive. This analysis explores when and where upsets tend to happen, and how they differ from non-upset matches.

**Main Research Question:** What patterns are associated with upset matches in the 2025 ATP Tour?

---

## ❓ Research Questions

| # | Question |
|---|----------|
| Q1 | How common were upset matches in the 2025 ATP Tour? |
| Q2 | Did upset rates vary by surface, tournament level, or round? |
| Q3 | Were upset matches different from non-upset matches in duration or performance patterns? |
| Q4 | How large were upset wins, and in which contexts did the biggest upsets happen? |

---

## 📊 Dataset

- **Source:** [TennisMyLife Tennis Match Database](https://stats.tennismylife.org/tennis-match-database)
- **Scope:** 2025 ATP Tour matches
- **Size:** 2,944 matches × 50 variables
- **Key Variables:** Player rankings, tournament level, surface, round, match duration, serve statistics

> ⚠️ Note: This is a public third-party dataset, not an official ATP source. It is used here for academic purposes only.

---

## 🛠 Tools & Libraries

- **Language:** Python 3
- **Environment:** Google Colab / Jupyter Notebook
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`

---

## 📂 Repository Structure

```
ATP-Upset-Analysis/
├── README.md
├── AliceLee_MESA8411_FinalProject_ATP2025.ipynb   # Main analysis notebook
├── AliceLee_MESA8411_FinalProject_Outline.docx    # Project outline
└── data/
    └── atp_matches_2025.csv                        # Dataset (download link above)
```

---

## 🚀 How to Run

**Option 1 – Google Colab (Recommended)**
1. Upload `atp_matches_2025.csv` to your Google Drive under `MyDrive/MESA8411/`
2. Open the `.ipynb` file in [Google Colab](https://colab.research.google.com/)
3. Run all cells

**Option 2 – Local Jupyter**
1. Clone this repository
2. Download the dataset from [TennisMyLife](https://stats.tennismylife.org/tennis-match-database)
3. Place the CSV in the same folder as the notebook
4. Update the file path in the notebook and run

---

## 🔍 Key Findings

### Q1. How common were upset matches?
- Out of **2,882 matches** with complete ranking data, **1,033 were upsets** — about **35.8% of all matches**
- Upsets were not rare; more than 1 in 3 matches ended with the lower-ranked player winning

### Q2. Did upset rates vary by surface, tournament level, or round?
- **Surface:** Grass had the highest upset rate, but differences across grass, hard, and clay were small — surface alone didn't strongly predict upsets
- **Tournament level:** **ATP 250 events consistently showed the highest upset rates**, while ATP 500 and Grand Slams were lower — tournament level was a stronger predictor than surface
- **Round:** Upset rates were highest in **R128 (first round)** and gradually declined in later rounds, though the differences weren't dramatic across most rounds

### Q3. Were upset matches different in duration or performance?
- **Match duration:** Upset matches lasted **longer on average** than non-upset matches, suggesting upsets tend to happen in more competitive matches
- **Rank gap:** Upset matches occurred at **smaller ranking gaps** — most upsets happened between players who were relatively close in ranking, not extreme mismatches
- **Aces:** Upset winners still had more aces than their opponents, but the advantage was smaller than in non-upset matches
- **Double faults:** No meaningful difference between upset and non-upset matches

### Q4. How large were the biggest upsets?
- The **median rank gap** in upset matches was ~42, but the **mean was ~83** — the distribution is right-skewed, driven by a few extreme upsets
- The largest upsets were concentrated in **Davis Cup and round-robin** matches (different competition format with wider ranking variation)
- Among standard ATP tour matches, the biggest upsets occurred across all three surfaces (hard, clay, grass)
- **ATP Finals** upsets had the smallest rank gaps, reflecting how closely ranked those players are

---

## ⚠️ Limitations

- Rankings alone do not capture player form, fatigue, injury, or head-to-head history
- Dataset is a third-party source and may have occasional gaps in serve statistics
- Analysis is limited to the 2025 season

---

## 📬 Contact

Feel free to reach out via GitHub if you have questions or suggestions!
