# Is NFL Week 1 Chaotic?

## Overview

This project investigates whether NFL Week 1 is unusually unpredictable when compared with the rest of the regular season. This is a work in progress.

## Research Questions

1. **Is Week 1 more upset-heavy than the rest of the regular season?**
2. **Are Week 1 games statistically different from games in Weeks 2–18?**
3. **Do team characteristics observed in Week 1 persist throughout the season?**

## Data

The project combines two primary data sources:

* **NFL game and team statistics:** `nflreadpy`
* **NFL betting data:** Spreadspoke's `nfl-scores-and-betting-data` dataset on Kaggle

The analysis covers regular-season games from **2006–2025**.

## Key Findings

### Week 1 Upsets

Week 1 does not appear to be significantly more upset-heavy than the rest of the regular season.

* Betting-market upset rate: **35.31%**
* Record-based upset rate: **35.13%**
* Record-based upset rate in Weeks 2–18: **36.24%**
* Difference: **−1.12 percentage points**
* 95% CI: **−6.94 to +4.71 percentage points**
* p-value: **0.709**

Large upsets were also examined using point spreads and differences in subsequent-season records.

### Week 1 Game Characteristics

Several aspects of Week 1 gameplay differed significantly from later games, particularly:

* Total penalties
* Total penalty yards
* Rushing yards
* Yards per rush

Passing production and several other game-level statistics showed little evidence of a Week 1 difference.

### Persistence of Week 1 Performance

Week 1 team performance showed statistically significant correlations with performance during Weeks 2–18. 

Production measures such as passing yards, offensive points, and rushing yards showed stronger persistence than several efficiency-based measures.

## Project Structure

The notebooks are organized as follows:

* **01_data_preparation.ipynb** — Loads, cleans, validates, and prepares the datasets.
* **02_upset_analysis.ipynb** — Defines and analyzes NFL upsets and addresses the first research question.
* **03_statistical_analysis.ipynb** — Examines Week 1 game characteristics and the persistence of team performance throughout the season.
