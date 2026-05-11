# Decades of Dominance: F1 Constructor Championship Performance, 1990–2024

![Tableau](https://img.shields.io/badge/Tableau-Public-blue) ![Data](https://img.shields.io/badge/Data-35%20Seasons-orange) ![Constructors](https://img.shields.io/badge/Constructors-4-red)

An interactive Tableau dashboard analysing the championship performance of Formula 1's four most successful constructors — Ferrari, McLaren, Mercedes, and Red Bull — across 35 seasons of competition.

🔗 **[View Live Dashboard on Tableau Public](#)** ← *replace with your link*

---

## Dashboard Preview

!images/Screenshot 2026-05-11 at 15.30.48.png
---

## Key Insights

- **Four distinct eras of dominance emerge clearly in the data.** McLaren led the 1990s (100 normalised score in 1990–1993), Ferrari dominated 1994–2004, Mercedes ran an unbroken streak from 2014–2021, and Red Bull have led since 2022 — with their 2023 season (10,158 points) representing the highest raw total in the dataset.

- **2024 marks the most competitive season in 35 years.** Ferrari (92.6) and McLaren (91.7) both achieved normalised scores above 90 for the first time since 2003, while Red Bull retained the lead — suggesting a genuine four-way title fight is emerging for the first time since the early 2000s.

- **Year-on-year volatility reveals how sharply performance can shift.** Ferrari's 2019 season saw the largest single-season points gain in the dataset (+4,450 points, +346%), while McLaren's 2023 drop (-5,398 points, -68%) was the steepest decline — illustrating how quickly regulation changes and technical failures can reshape the competitive order.

---

## Dataset

| Field | Description |
|---|---|
| `constructor` | Team name (Ferrari, McLaren, Mercedes, Red Bull) |
| `season` | Championship year (1990–2024) |
| `total_points` | Total constructors' championship points for the season |
| `points_normalised` | Points scaled 0–100 relative to the season leader |
| `prev_points` | Prior season points (used to calculate YoY change) |
| `yoy_change` | Absolute points change vs. prior season |
| `yoy_change_pct` | Percentage points change vs. prior season |

**Note on normalisation:** Raw points are not directly comparable across seasons due to rule changes (e.g. double points, sprint races). The `points_normalised` field benchmarks each constructor against the season leader to enable fair cross-era comparison.

**Source:** [Ergast F1 API](http://ergast.com/mrd/) / [Formula 1 official results](https://www.formula1.com/en/results)

---

## Dashboard Features

- **Points Over Time** — line chart tracking all four constructors across 35 seasons, colour-coded by team
- **Year-on-Year Change** — diverging bar chart showing season-on-season points movement, with a zero reference line
- **Normalised Performance** — relative benchmarking view allowing cross-era comparison despite changing scoring systems
- **Interactive Filters** — constructor selector and season range slider to explore specific teams and eras

---

## Tools Used

- **Tableau Public** — dashboard design and visualisation
- **Excel / Python** — data cleaning and feature engineering (YoY change, normalisation)

---

## How to Use

1. Open the [live dashboard](#) on Tableau Public
2. Use the constructor checkboxes to isolate specific teams
3. Drag the season slider to focus on a particular era
4. Hover over any data point for detailed tooltip information

---

## About

This project is part of my data analytics portfolio. I'm a career-changer transitioning from hospitality management, where I worked extensively with revenue forecasting and performance data. This project demonstrates my ability to source, clean, and visualise longitudinal data to surface meaningful trends.

📂 [Back to Portfolio](../)
