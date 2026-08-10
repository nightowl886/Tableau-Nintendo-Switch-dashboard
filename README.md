# Tableau Nintendo Switch dashboard 
🎮 Nintendo Switch Tableau Dashboard
## 📖 Overview
This project analyzes Nintendo Switch video game data and visualizes trends in releases, ratings, reviews, and publisher performance using Tableau. The goal is to demonstrate skills in data cleaning, SQL preparation, and interactive dashboard design.

## 📂 Project Structure

```
nintendo-switch-dashboard/
│
├── data_cleaning.sql       # SQL script for cleaning raw data
├── cleaned_data.csv        # Final dataset used in Tableau
├── tableau/                # Tableau workbook files
│   └── dashboard.twbx
└── README.md               # Project documentation

```

## 🛠️ Workflow

### 1. Data Cleaning

- Remove duplicates, handle missing values, and standardize formats.

- Export cleaned dataset for Tableau.

### 2. Initial Visualization & Date Formatting in Tableau
-During the initial visualization stage, Tableau’s default date parser could not interpret release dates containing ordinal suffixes (e.g., 1st, 2nd, 3rd, 4th). This caused errors in chronological sorting and prevented accurate quarterly analysis.

-✅ Solution
I created a calculated field in Tableau that explicitly checks for each suffix (st, nd, rd, th) and parses the date accordingly. This ensured all release dates were converted into valid DATE values.

Releases by Quarter  
Timeline of game releases across quarters.

Strongest & Weakest Performers  
Bar charts comparing top-rated and lowest-rated games.

Publisher Quality  
Scatter plots showing average ratings vs. release volume.

Doughnut Chart  
Genre distribution or publisher market share.

Image URL Placement  
Display game cover images dynamically.

Dynamic Game Info  
Interactive display of ratings, reviews, and release details.

Votes & Reviews  
Visualize relationship between number of reviews and ratings.

URL Actions  
Click-through links to external sources (e.g., Metacritic).

Tooltips & Formatting  
Final polish: tooltips, layout, and design consistency.

Conclusion  
Wrap-up and key insights.

📊 Dashboard Highlights
Quarterly release trends

Top & bottom performers

Publisher quality analysis

Interactive cover images and dynamic info display

URL actions for external references

Clean, professional formatting with tooltips

🚀 How to Use
Run data_cleaning.sql to prepare the dataset.

Load cleaned_data.csv into Tableau.

Open dashboard.twbx to explore the interactive dashboard.

📌 Deliverables
SQL scripts for data preparation

Clean dataset for reproducibility

Interactive Tableau dashboard with multiple visualizations

README documentation with workflow and screenshots
