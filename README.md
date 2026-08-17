# Tableau Nintendo Switch Dashboard 
🎮 Nintendo Switch Tableau Dashboard
## 📖 Overview
This project analyzes Nintendo Switch game data and visualizes key trends in releases, ratings, publisher behavior, and player engagement using Tableau. The dashboard highlights **how many games Nintendo releases each quarter**, identifies the **Top 10 strongest and weakest performers**, evaluates the **quality of frequent publishers**, and includes an **interactive game detail panel** that displays dynamic information when a user selects a specific title.

The interactive dashboard allows users to explore:

- Quarterly release patterns across the Nintendo Switch catalog

- Top 10 highest‑rated and lowest‑rated games, filtered to ensure reliability (only titles with more than 200 reviews are included)

- Detailed game information on click, including cover image, number of reviews, rating score, and a short description
  
- Quality of Frequent Publishers

This project demonstrates skills in data cleaning, visualization design, and building interactive Tableau experiences that combine statistical rigor with user‑friendly exploration.

Together, these visualizations provide a comprehensive, interactive view of the Nintendo Switch game ecosystem, combining release trends, performance rankings, publisher quality, and detailed game‑level insights.



## 📂 Project Structure

```
nintendo-switch-dashboard/
│
├── switch-games.xlsx        # Final dataset used in Tableau
├── tableau/                # Tableau workbook files
│   └── Nintendo Switch.twb
│   └── interactive Dashboard.mov
│   └── Tableau Dashboard.png
└── README.md               # Project documentation

```

## 🛠️ Workflow

### 1. Data Cleaning

- Remove duplicates, handle missing values, and standardize formats.

- Export cleaned dataset for Tableau.

### 2. Initial Visualization & Date Formatting in Tableau
- During the initial visualization stage, Tableau’s default date parser could not interpret release dates containing ordinal suffixes (e.g., 1st, 2nd, 3rd, 4th). This caused errors in chronological sorting and prevented accurate quarterly analysis.

- ✅ Solution: \
I created a calculated field in Tableau that explicitly checks for each suffix (st, nd, rd, th) and parses the date accordingly. This ensured all release dates were converted into valid DATE values.

### 3. Quarterly Release Trends  
- A time‑series visualization showing how many Nintendo Switch games were released each quarter.
- Helps identify publishing cycles, seasonal spikes, and long‑term trends.

### 4. Strongest & Weakest Performers  
- Bar charts comparing the **Top 10 strongest performers** and **Top 10 weakest performers** across all Nintendo Switch games.
- To ensure rankings are high-engagement and trustworthy, a filter was applied: only games with more than 200 votes (num_votes > 200) are eligible.
- This prevents titles with inflated ratings but very few votes from appearing in the Top 10 lists.
- The final charts highlight both consistently high‑rated titles and reliably low‑rated titles based on sufficient community engagement.

### 5. Interactive Game Details
- The dashboard includes an interactive panel that displays detailed information when a user clicks on any game.

- The dynamic display shows:

  - Game cover image

  - Number of reviews

  - Rating score

  - Short game description/summary

- This interaction allows users to explore individual titles without leaving the dashboard, creating a more immersive and user‑friendly exploration experience.

### 6. Quality of Frequent Publishers  
- A bubble chart comparing publishers by both release volume and average rating.
- This highlights which publishers consistently deliver high‑quality titles and which ones release many lower‑rated games.

---
## 📊 Dashboard Highlights


- Quarterly release trends

- Top & bottom performers

- Publisher quality analysis

- Interactive cover images and dynamic info display

- URL actions for external references

- Clean, professional formatting with tooltips

## 📌 Deliverables

- Clean dataset for reproducibility

- Interactive Tableau dashboard with multiple visualizations

- README documentation with workflow and screenshots
  
- Tableau Dashboard Visualization
  https://public.tableau.com/views/NitendoSwitch/Dashboard?:language=zh-CN&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

