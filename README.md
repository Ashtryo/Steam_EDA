<div align="center">

<img src="https://upload.wikimedia.org/wikipedia/commons/8/83/Steam_icon_logo.svg" width="120">

# Steam Games EDA & Visualization Project
### Exploratory Data Analysis of Steam Marketplace Data
**By:** Ansh Bansal

</div>

---

## 📑 Table of Contents
1. [Project Objective](#-project-objective)
2. [Dataset Overview](#-dataset-overview)
3. [Tech Stack](#-tech-stack)
4. [A to Z EDA Process (Step-by-Step)](#-a-to-z-eda-process-step-by-step)
5. [Key Questions Answered (Visualizations)](#-key-questions-answered-visualizations)
6. [Major Findings & Conclusions](#-major-findings--conclusions)
7. [Strategic Business Recommendations](#-strategic-business-recommendations)
8. [How to Run This Project](#-how-to-run-this-project)

---

## 🎯 Project Objective
The core objective of this project is to analyze Steam games data to thoroughly understand pricing, reviews, genres, developers, publishers, and overall platform trends. This analysis is designed to uncover business insights that can help game developers and publishers make better data-driven decisions.

---

## 📊 Dataset Overview
This dataset contains extensive information about games available on the Steam platform, including game details, pricing, review metrics, hardware requirements, and user-generated tags. 

### Data Dictionary
| Column | Description |
| :--- | :--- |
| **Appid** | Unique Steam application ID for each game |
| **Name** | Name of the game |
| **Type** | Type of Steam product (Game, DLC, etc.) |
| **ReleaseDate** | Official release date of the game |
| **Genres** | Genres associated with the game |
| **Developers** | Developer(s) of the game |
| **Publishers** | Publisher(s) of the game |
| **Description** | Store description of the game |
| **price** | Current price of the game |
| **Thumbnail** | URL of the game's thumbnail image |
| **Tags** | User-generated tags describing the game |
| **ReviewScore** | Overall review score category |
| **PositiveReview** | Number of positive reviews |
| **NegativeReview** | Number of negative reviews |
| **OsRequirement** | Operating system requirements |
| **MemoryRequirement**| RAM requirement |
| **CpuRequirement** | Processor requirement |
| **Rank** | Steam ranking or popularity indicator |

---

## 💻 Tech Stack
* **Language:** Python
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `re` (Regular Expressions)

---

## 🛠️ A to Z EDA Process (Step-by-Step)
The following data cleaning and feature engineering steps were executed in exact notebook order to ensure data integrity:

1. **Import libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `re`.
2. **Load dataset** from `SteamGames.csv` into a dataframe.
3. **Initial peek:** Utilized `head()`, `tail()`, and `sample()` for an unbiased understanding.
4. **Structure checks:** Reviewed `shape`, `columns`, `info()`, and `describe()`.
5. **Missing & duplicates:** Checked with `isnull().sum()` and `duplicated().sum()`.
6. **Drop unnecessary columns:** Removed the `Thumbnail` column as it does not contribute to the analysis.
7. **Clean data:** Removed '$' from `price` and converted it to float; parsed `ReleaseDate` into datetime.
8. **Drop missing values:** Removed rows missing `ReleaseDate`.
9. **Filter products:** Filtered `Type` to keep only `game` and `dlc`.
10. **Drop missing categories:** Dropped rows missing `Genres`.
11. **Fill missing metadata:** Filled missing `Developers`, `Publishers` with "Unknown", and provided placeholders for missing `Description` and `Tags`.
12. **Normalize text data:** Standardized OS requirements using dictionary replacements and a complex normalization function utilizing regular expressions.
13. **Fill missing hardware requirements:** Filled `MemoryRequirement` and `CpuRequirement` with 'Not Specified'.
14. **Feature engineering:** Created highly actionable features including `TotalReviews`, `ReleaseYear`, `ReleaseMonth`, `IsFree`, `Pos_Ratio`, and `ReleaseDay`.
15. **Export:** Saved the cleaned dataset to `Cleaned_SteamGames.csv`.

---

## 🔍 Key Questions Answered (Visualizations)
During the exploratory data analysis phase, several critical market questions were addressed:

* **What is the standard distribution of game prices?** Most games are priced under $10.
* **What proportion is Free-to-Play?** 15-20% of games are free.
* **Does making a game more expensive lead to harsher reviews?** Yes, the variance in positive reviews widens as prices approach $60.
* **How is player attention distributed?** Steam is a "Winner-Takes-All" economy where a tiny fraction captures 90% of reviews.
* **Do Free games get better reviews than Paid games?** Paid games usually score better, as Free games are prone to review bombing.
* **Has release volume increased?** Yes, the market exploded after 2014, leading to hyper-saturation.
* **Which month/day is most competitive?** October and November are the most congested months. Tuesday and Thursday dominate release days.
* **What are the most saturated genres?** "Action", "Indie", and "Adventure".
* **Which genres generate the most total revenue?** "Action" and "RPG".
* **Do Multiplayer games command a higher price?** Yes, the inclusion of multiplayer servers allows developers to charge a higher premium.
* **How have minimum RAM requirements evolved?** They shifted from 2GB in 2010 to an average minimum of 7GB by 2024.

---

## 🏆 Major Findings & Conclusions

### 1. Market Saturation & Pricing Dynamics
* **Winner-Takes-All Reality:** A handful of viral hits capture nearly all player attention, leaving most titles overlooked.
* **Crowded Low-Price Tier:** The market under $10 is crowded. Breaking into the $20+ premium tier requires strong marketing or an established IP.
* **Revenue Concentration:** Most estimated revenue comes from titles priced between $30–$60.

### 2. Player Sentiment & Reviews
* **Premium Punishment:** At the $60 AAA tier, players are far less forgiving of bugs and issues.
* **Early Access Forgiveness:** Players cut developers slack when a game is labeled *Early Access*, tolerating bugs as a work-in-progress.

### 3. Genre & Mechanics Insights
* **Saturated vs. Lucrative:** While *Indie* has the highest game count, *Action* and *RPG* dominate actual revenue.
* **Singleplayer Demand:** *Singleplayer* remains the most common user tag.

### 4. Temporal & Release Trends
* **No Weekend Rule:** Developers avoid weekends to catch press outlets and Steam’s algorithm during business hours.
* **Hardware Evolution:** Minimum RAM requirements have steadily climbed—from 2GB (2010) to ~7GB (2024).

---

## 💡 Strategic Business Recommendations
Based on the data, here is a strategic blueprint for success on Steam:

1. **Optimize Release Timing:** Avoid October–November if you are indie or mid-sized. Launch in Q1 or Q2 for better visibility, specifically on a Tuesday or Thursday.
2. **Target the Golden Revenue Formula:** Aim for the $30–$60 tier and blend Action + RPG mechanics with Multiplayer/Co-op to maximize returns.
3. **Set Modern Hardware Baselines:** Stop optimizing for outdated 4GB RAM machines; design with 8GB RAM as the minimum baseline.
4. **Use Early Access Wisely:** If QA resources are limited, launch in Early Access to shield your rating while fixing bugs.
5. **Quality & Brand > Quantity:** Flooding the market doesn't guarantee success. Focus on polished games and building a strong brand reputation.

---

## 🚀 How to Run This Project

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yourusername/Steam-Market-EDA.git](https://github.com/yourusername/Steam-Market-EDA.git)
