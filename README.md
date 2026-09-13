# netflix-viewership-analysis
Relational data analysis using Python to optimize Netflix's content release and acquisition strategy.
# 🎬 Netflix Multi-Table Data Analysis & Content Strategy

## 🧑‍💻 Analyst: Olga Mikirtumova

---

## 📌 Executive Summary & Key Recommendations
*   **Target Q4 for Major Drops:** Historical viewership trends show a massive seasonal surge at the end of the year. To optimize ROI, Netflix's highest-budget releases should be heavily scheduled for Q4.
*   **Optimize Catalog Efficiency with TV Shows:** Despite having a catalog half the size of movies, TV shows achieve highly competitive viewership numbers (~505K views per title vs. ~529K for movies) and nearly match them in audience satisfaction scores. Expanding the TV show footprint is a cost-effective vehicle for user engagement.
*   **Prioritize Audience Reach Over Critical Acclaim:** Viewership data shows virtually no correlation with user ratings. Strategic content acquisition should prioritize popular genres (Sci-Fi, Comedy, Musical) rather than high user review metrics.

---

## 📖 Project Overview
This project explores Netflix's catalog, user ratings, and viewership metrics across 5 relational tables (`titles`, `genres`, `cast`, `ratings`, and `viewership`). The objective is to evaluate data integrity, clean and structure the relational matrices, uncover content performance insights, and deliver actionable recommendations to the executive content team.

## 🛠️ Tech Stack & Tools
*   **Language:** Python 3.11
*   **Libraries:** 
    *   `pandas` (Relational merges, data manipulation, type casting)
    *   `numpy` (Numerical operations)
    *   `matplotlib.pyplot` & `seaborn` (Advanced data visualization)
*   **Environment:** Jupyter Notebook

---

## 📊 Core Analytical Findings

### 🎥 1. Catalog & Demographics Overview
*   **The Size Imbalance:** Netflix's library contains **800 unique titles**. The catalog of film titles is twice as large as the television catalog.
*   **Target Audiences:** Family-friendly and general-audience material heavily dominates the service, with **TV-PG** tracking as the platform's most frequent content rating.
*   **Global Production Hubs:** **Australia, Nigeria, and Japan** lead the library as the top 3 contributing production countries outside of unknown regions.

### 🎭 2. Content Dynamics & Talent
*   **Top Genres:** The most common genre tags found throughout the library are **Comedies, Documentaries, and Stand-Up Comedies**. 
*   **Format Preferences:** Documentaries and Romantic Movies dominate the movie catalog, whereas Comedies and Independent titles lead the TV show division.
*   **Star Power:** **Penélope Cruz** is the platform's most frequent actor, clinching the #1 rank for leading roles, while tying with Ken Watanabe for the most supporting roles.

### 📈 3. Viewership & Ratings Trends
*   **Platform Baseline:** User reception is broadly stable and positive, keeping the platform's overall average rating at **3.64 out of 5**.
*   **Genre Preferences:** While Dramas, LGBTQ, and Romantic Movies capture the highest average star ratings, **Sci-Fi & Fantasy, Comedies, and Music & Musicals** generate the highest absolute view counts.
*   **The Ratings Illusion:** Scatterplot analysis reveals **no significant correlation** between high user ratings and high view counts, establishing that critical or user satisfaction metrics do not organically drive platform popularity.

---

## 🚀 Concrete Content Strategy Recommendations

### 1. Optimize High-Budget Release Windows
*   **Action:** Schedule your biggest and most capital-intensive releases exclusively for the final months of the year, while actively avoiding major drops during the summer season.
*   **Data Backing:** Cross-platform monthly viewership data indicates that engagement predictably dips during mid-year summer months as outdoor activity rises, and peaks significantly in Q4 as winter seasons and holidays begin. 

### 2. Implement a Tiered Genre Investment Strategy
*   **Action:** Allocate top-tier development budgets to the **Sci-Fi & Fantasy** category to serve as the main anchor for platform retention. Utilize **Comedies** and **Music & Musicals** as foundational bridge content, strategically staggered between major Sci-Fi releases.
*   **Data Backing:** While Sci-Fi & Fantasy brings in the highest aggregate volume of viewers, Comedies and Musicals rank close behind as the second and third most-viewed categories on the platform, providing the most reliable constant audience reach.

### 3. Strategically Expand the TV Show Library
*   **Action:** Allocate a higher percentage of the acquisition and licensing budget toward episodic TV shows to reduce reliance on expanding the movie library.
*   **Data Backing:** Despite having a catalog footprint half the size of movies, individual TV shows pull highly competitive viewership numbers (~505K views per title) compared to movies (~529K). Furthermore, TV shows hold practically identical average customer review ratings to movies (3.61 vs. 3.66). Expanding this format offers a highly efficient path toward growing long-term platform engagement.

---

## 📂 Repository Structure

*   `analysis/`: Contains the end-to-end Python data pipeline, spanning missing value imputation, date conversions, relational table joins, and fully optimized data visualization code.
*   `data/`: Data architecture files housing the original relational CSV files (`titles`, `genres`, `cast`, `ratings`, `viewership`).
