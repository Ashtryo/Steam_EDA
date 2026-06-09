# 🎮 Steam Games Market Analysis & Exploratory Data Analysis

<div align="center">

<img src="https://upload.wikimedia.org/wikipedia/commons/8/83/Steam_icon_logo.svg" width="120">

## Comprehensive Exploratory Data Analysis of Steam Marketplace Data

### By Ansh Bansal

</div>

---

# 📌 Project Overview

The gaming industry has become one of the largest entertainment industries in the world, with Steam being the dominant digital distribution platform for PC games.

This project performs a complete Exploratory Data Analysis (EDA) on Steam games data to uncover insights related to pricing, reviews, genres, developers, publishers, release patterns, hardware requirements, and overall marketplace trends.

The goal of this analysis is to transform raw Steam marketplace data into actionable business insights that can help developers, publishers, analysts, and gaming businesses make informed decisions.

---

# 📥 Dataset

Due to GitHub file size limitations, the dataset is not included directly in this repository.

### Download Dataset

https://drive.google.com/file/d/1xW072PyFU94Xc1EeHz1Cbg7vtjIxj_zE/view?usp=drive_link

After downloading, place the dataset in the project root directory:

Steam-Games-EDA/

├── SteamGames.csv

├── STEAM_ANALYSIS.ipynb

├── README.md

---

# 📑 Table of Contents

1. Project Objective
2. Dataset Overview
3. Project Preview
4. Tech Stack
5. Data Cleaning & Preprocessing
6. Feature Engineering
7. Exploratory Data Analysis
8. Key Questions Answered
9. Major Findings
10. Business Recommendations
11. Skills Demonstrated
12. Future Improvements
13. Project Structure
14. Installation & Usage

---

# 🎯 Project Objective

The primary objective of this project is to analyze Steam marketplace data and identify meaningful patterns in:

* Game Pricing
* User Reviews
* Genre Popularity
* Publisher Performance
* Developer Trends
* Release Behavior
* Hardware Requirements
* Free-to-Play Growth
* Multiplayer Adoption

The project aims to answer important business questions using data-driven analysis and visualizations.

---

# 📊 Dataset Overview

### Dataset Information

| Metric   | Value                  |
| -------- | ---------------------- |
| Records  | ~29,931 Games          |
| Features | 18 Columns             |
| Domain   | Gaming Industry        |
| Source   | Steam Marketplace Data |

### Dataset Columns

| Column            | Description           |
| ----------------- | --------------------- |
| Appid             | Unique Steam Game ID  |
| Name              | Game Name             |
| Type              | Product Type          |
| ReleaseDate       | Release Date          |
| Genres            | Game Genres           |
| Developers        | Developer Information |
| Publishers        | Publisher Information |
| Description       | Game Description      |
| Price             | Game Price            |
| Thumbnail         | Thumbnail URL         |
| Tags              | Steam User Tags       |
| ReviewScore       | Review Category       |
| PositiveReview    | Positive Reviews      |
| NegativeReview    | Negative Reviews      |
| OsRequirement     | OS Requirement        |
| MemoryRequirement | RAM Requirement       |
| CpuRequirement    | CPU Requirement       |
| Rank              | Steam Ranking         |

---

# 📸 Project Preview

Add your best visualization screenshots here.

Example:

![Price Distribution](https://github.com/Ashtryo/Steam_EDA/blob/main/images/output%202.png)

![Genre Analysis](images/genre_analysis.png)

![Review Analysis](images/review_analysis.png)

![Correlation Heatmap](images/correlation_heatmap.png)

---

# 💻 Tech Stack

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Regular Expressions (re)

### Tools

* Jupyter Notebook
* Git
* GitHub

---

# 🧹 Data Cleaning & Preprocessing

The dataset was cleaned and transformed through the following steps:

1. Imported required libraries
2. Loaded Steam dataset
3. Performed initial exploration
4. Checked dataset structure
5. Identified missing values
6. Identified duplicate records
7. Removed unnecessary columns
8. Cleaned price column
9. Converted release dates to datetime
10. Filtered valid game types
11. Handled missing genres
12. Filled missing developer information
13. Filled missing publisher information
14. Standardized operating system requirements
15. Normalized text fields
16. Filled missing hardware requirements
17. Exported cleaned dataset

---

# ⚙️ Feature Engineering

Several new analytical features were created:

### Total Reviews

TotalReviews = PositiveReview + NegativeReview

Used to measure player engagement.

### Review Positivity Ratio

Pos_Ratio = PositiveReview / TotalReviews

Used to estimate player satisfaction.

### Release Features

* ReleaseYear
* ReleaseMonth
* ReleaseDay

### Free-to-Play Flag

IsFree

Used to separate paid and free games.

### Revenue Proxy

Revenue_Proxy = Price × TotalReviews

Used as an estimated commercial performance metric.

Note: This is not actual revenue.

---

# 📈 Exploratory Data Analysis

The notebook investigates multiple business and market questions through visualizations and statistical analysis.

Major areas analyzed:

* Price Distribution
* Review Distribution
* Revenue Patterns
* Genre Analysis
* Publisher Analysis
* Developer Analysis
* Release Trends
* Free-to-Play Growth
* Multiplayer Trends
* Early Access Analysis
* Hardware Evolution
* Correlation Analysis

---

# 🔍 Key Questions Answered

### Pricing Analysis

* What is the distribution of game prices?
* What percentage of games are free?

### Review Analysis

* Do expensive games receive better reviews?
* How are reviews distributed?

### Market Analysis

* How has Steam grown over time?
* Which genres dominate the platform?

### Business Analysis

* Which genres generate the highest revenue potential?
* Which publishers dominate the marketplace?

### Technical Analysis

* How have RAM requirements evolved?
* How have hardware requirements changed?

---

# 🏆 Major Findings

### Market Insights

* Most Steam games are priced below $10.
* Free-to-Play games represent a significant share of the platform.
* Steam releases increased dramatically after 2014.

### Customer Insights

* Most player attention is concentrated among a small number of games.
* Higher prices do not automatically guarantee better reviews.
* Early Access titles often maintain strong positivity ratios.

### Genre Insights

* Action, Adventure, RPG, and Indie dominate the platform.
* Action and RPG genres show strong commercial potential.

### Technical Insights

* RAM requirements have increased steadily over time.
* Modern games require significantly more hardware resources.

---

# 💡 Strategic Business Recommendations

### 1. Release Timing

Avoid highly competitive launch periods when possible and analyze seasonal release patterns before publishing.

### 2. Pricing Strategy

Carefully position products in premium tiers only when sufficient value is delivered.

### 3. Genre Selection

Combine high-demand genres with strong market potential.

### 4. Multiplayer Features

Multiplayer functionality can increase perceived value and pricing flexibility.

### 5. Early Access Strategy

Use Early Access strategically to gather feedback and improve product quality.

---

# 📈 Key Results Summary

| Analysis Area      | Key Finding                 |
| ------------------ | --------------------------- |
| Price Distribution | Most games priced below $10 |
| Free Games Share   | Significant market presence |
| Genre Leader       | Action                      |
| Revenue Potential  | Action & RPG                |
| Market Growth      | Rapid expansion after 2014  |
| Hardware Trend     | RAM requirements increasing |

---

# 🎓 Skills Demonstrated

* Data Cleaning
* Data Wrangling
* Exploratory Data Analysis
* Feature Engineering
* Statistical Analysis
* Data Visualization
* Business Analytics
* Python Programming
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

# 🔮 Future Improvements

Potential future enhancements include:

* Revenue Prediction Models
* Review Score Prediction
* Steam Recommendation System
* Interactive Dashboard (Power BI/Tableau)
* Market Trend Forecasting
* Machine Learning Applications

---

# 📁 Project Structure

Steam-Games-EDA/

├── SteamGames.csv

├── STEAM_ANALYSIS.ipynb

├── README.md

├── requirements.txt

└── images/

    ├── price_distribution.png

    ├── genre_analysis.png

    ├── review_analysis.png

    └── correlation_heatmap.png

---

# 🚀 Installation & Usage

### Clone Repository

git clone https://github.com/yourusername/Steam-Games-EDA.git

### Navigate to Project

cd Steam-Games-EDA

### Install Dependencies

pip install pandas numpy matplotlib seaborn

### Run Jupyter Notebook

jupyter notebook

Open:

STEAM_ANALYSIS.ipynb

and run all cells sequentially.

---

# 👨‍💻 Author

Ansh Bansal

Aspiring Data Analyst passionate about transforming raw data into meaningful business insights through analytics, visualization, and data-driven decision making.

---

# ⭐ Support

If you found this project useful, please consider giving it a star.

Star ⭐ the repository if you learned something from this analysis.
