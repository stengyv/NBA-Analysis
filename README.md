# NBA 2024-25 Season Performance Analysis

An exploratory data analysis (EDA) project examining team and game-level performance 
across the 2024-25 NBA season to identify which statistics are most strongly associated 
with winning.

## Overview

This project collects data directly from the NBA API, aggregates 2,460+ game records 
across all 30 teams, and analyzes the relationships between various performance metrics 
and game outcomes.

## Key Findings

- **Offensive efficiency** (FG_PCT, PTS) showed the strongest positive correlation with winning
- **Turnovers** (TOV) showed the strongest negative correlation with winning
- Teams with better ball control consistently posted higher win percentages

## Tools & Libraries

- Python
- pandas
- seaborn
- matplotlib
- nba_api

## Files

| File | Description |
|------|-------------|
| `nba_analysis.ipynb` | Main analysis notebook |
| `nba_gamelogs.csv`   | Raw game-level data (2,460 rows) |
| `nba_averages.csv`   | Team-level season averages (30 rows) |

## How to Run

1. Install dependencies: `pip install nba_api pandas seaborn matplotlib`
2. Open `nba_analysis.ipynb` in VS Code with the Jupyter extension installed

> **Note:** The data collection cell makes API calls for all 30 teams and includes 
> a 1-second delay between requests to avoid rate limiting. Expect it to take ~1 minute to run.
