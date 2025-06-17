#  Video Game Sales Market Analysis

This Jupyter Notebook explores historical video game sales data to identify the factors that contribute to a game's commercial success. The project was completed as part of a data analysis course and simulates preparing for a 2017 marketing campaign.

##  Project Overview

- **Client**: Strimchik — an online video game retailer with a global customer base.
- **Objective**: To identify key patterns that influence game sales, such as platform, genre, region, and review scores.
- **Dataset**: Provided as part of the Yandex Practicum Data Analyst course ([practicum.yandex](https://practicum.yandex)).
- **Time frame**: 1980–2016

##  Key Questions Answered

- How do game sales vary by year and platform?
- What platforms have been the most commercially successful in recent years?
- Do critic or user ratings affect sales?
- What are the most popular genres in different regions?
- How do North American, European, and Japanese markets differ?

##  Hypotheses Tested

1. **Null Hypothesis H₀**: The mean user ratings for Xbox One and PC are equal.  
   - **Result**: The null hypothesis **could not be rejected** (p-value > 0.05), indicating no statistically significant difference.

2. **Null Hypothesis H₀**: The mean user ratings for Action and Sports genres are equal.  
   - **Result**: The null hypothesis was **rejected** (p-value < 0.05), indicating a statistically significant difference in ratings between these two genres.

##  Methodology

- Data cleaning and preprocessing (handling missing values, fixing column types)
- Exploratory data analysis using pandas, matplotlib, and seaborn
- Hypothesis testing using `scipy.stats.ttest_ind`

##  Main Findings

- **PS4** was the top-selling platform globally from 2013 to 2016.
- **Critic scores** show a moderate correlation with sales, while **user scores** show virtually none.
- **Popular genres** vary slightly by region:
  - NA: Shooter, Action
  - EU: Action, Shooter
  - JP: Role-Playing
- Japanese players prefer different platforms and genres than Western audiences.
- ESRB “Mature” games dominate in NA and EU markets.

## 📁 File Structure

- `games_proj.ipynb` — Full analysis notebook
- `games.csv` — 

## 📦 Technologies Used

- Python 3
- pandas
- matplotlib
- seaborn
- scipy
- Jupyter Notebook

## 📎 Dataset Source

The dataset was provided as part of the Yandex Practicum “Data Analyst” course. It includes information on global game sales from 1980 to 2016 across multiple platforms.

## 🗂 How to Run

```bash
# Clone this repository
git clone https://github.com/yourusername/video-game-sales-analysis.git

# Install dependencies
pip install -r requirements.txt  # optional

# Launch the notebook
jupyter notebook games_project_final.ipynb
