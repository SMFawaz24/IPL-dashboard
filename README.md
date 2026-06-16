# IPL Dashboard (2008–2024)

An end-to-end data analytics project covering 17 seasons of the Indian Premier League — from raw data cleaning in Python to an interactive Power BI dashboard.

**Dataset scope:** 1,095 matches | 260,920 ball-by-ball deliveries | 2008–2024

---

## Dashboard Preview

### Overview 
<img width="898" height="506" alt="overview" src="https://github.com/user-attachments/assets/36bce028-5ec7-4b81-8792-d52b820c006a" />

### Teams
<img width="896" height="504" alt="teams" src="https://github.com/user-attachments/assets/77781fbf-041d-47da-9c66-e1be3b3e0d3a" />

### Batsmen
<img width="898" height="508" alt="batsmen" src="https://github.com/user-attachments/assets/44e6003d-585f-4ca7-9c85-116828fe26d9" />

### Bowlers
<img width="898" height="508" alt="bowlers" src="https://github.com/user-attachments/assets/05be5e1a-d461-40ed-900d-646419f38d41" />

### Venues
<img width="904" height="512" alt="venues" src="https://github.com/user-attachments/assets/b5f8a434-a6e7-4d2f-abb4-b01b19a14075" />

---

## Repository Structure

```
IPL-dashboard/
├── notebooks/              Jupyter notebooks — full data pipeline
├── screen_shots/           Dashboard screenshots
├── IPL Dashboard.pbix      Power BI dashboard
└── IPL_PowerBI_Data.xlsx   Cleaned, model-ready dataset
```

---

## Data Pipeline

The analysis is structured as a sequential pipeline of five notebooks:

| Notebook | Description |
|---|---|
| `01_data_cleaning.ipynb` | Standardizes season labels and team names, resolves missing values, and engineers derived fields (match phase, boundary flags, dot balls) |
| `02_eda_teams.ipynb` | Team-level analysis: win counts, win rates, toss impact, head-to-head records, and batting-first vs. chasing trends |
| `03_eda_players.ipynb` | Player performance: top run scorers, strike rate vs. average, leading wicket-takers, bowling economy, and phase-wise scoring patterns |
| `04_eda_venues.ipynb` | Venue analysis: matches hosted, average first-innings totals, chase success rates, and boundary frequency by ground |
| `05_export_for_powerbi.ipynb` | Consolidates all processed outputs into a single Excel workbook for Power BI |

---

## Dataset

Source: [IPL Complete Dataset (2008–2024), Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)

---

## Key Findings

- Virat Kohli is the all-time leading run scorer with 8,014 runs
- Mumbai Indians hold the highest win total in IPL history (144 wins)
- Winning the toss provides only a marginal advantage, with toss-winners winning ~50.6% of matches
- Average first-innings totals have risen sharply since 2022, approaching 190 runs
- Among bowlers with 300+ balls delivered, Yuzvendra Chahal leads with 205 wickets

---

## Tech Stack

- **Python**: pandas, numpy, matplotlib, seaborn
- **Power BI**: 5-page interactive dashboard featuring a custom dark theme, cross-page navigation, and dynamic slicers

---

## Getting Started

```bash
git clone https://github.com/SMFawaz24/IPL-dashboard.git
cd IPL-dashboard
pip install pandas numpy matplotlib seaborn openpyxl jupyter
jupyter notebook notebooks/01_data_cleaning.ipynb
```

Open `IPL Dashboard.pbix` in Power BI Desktop to explore the full dashboard.

---

## Author

[Syed Mohammad Fawaz](https://github.com/SMFawaz24)
