# Video Game Analysis: Identifying Success Patterns in the Global Market

This project analyzes historical video game sales data to identify patterns that determine commercial success, with the goal of guiding advertising campaigns and development strategies.

## Objective

To identify patterns that determine the success of a video game through the analysis of sales, popular platforms, profitable genres, and regional differences in consumption preferences.

## 🛠️ Technologies Used

*   **Python:** Primary language.
*   **Pandas, NumPy:** Data manipulation and analysis.
*   **Matplotlib, Seaborn:** Data visualization.
*   **SciPy:** Statistical hypothesis testing (Student's t-test).
*   **Jupyter Notebook:** Interactive development environment.

## Dataset

The dataset (`games.csv`) contains information on more than 16,000 video games released up to 2016, including name, platform, release year, genre, sales by region, critic and user scores, and ESRB rating.

## Key Analysis Steps

1.  **Data Preparation:** Cleaning missing values, standardizing formats, creating a `total_sales` column (sum of regional sales).

2.  **Exploratory Analysis:** Visualization of releases by year, identification of platforms with the highest total sales (PS2, X360, PS3, Wii), and analysis of platform life cycles (6-10 years).

3.  **Current Market Analysis (2012-2016):**
    *   **Leading platforms:** PS4, PS3, and X360 dominate; Sony leads the market, Nintendo has a smaller presence.
    *   **Sales distribution:** Boxplots show high dispersion and outliers (very successful games) on all platforms.
    *   **Impact of reviews:** Low to moderate correlation between scores and sales; reviews are not the only determining factor.
    *   **Profitability by genre:** Action is the most common genre, but shooters and sports are the most profitable per title.

4.  **User Profile by Region:**
    *   **NA and EU:** Dominated by home consoles (Xbox, PlayStation) and action and sports genres.
    *   **Japan:** Preference for handheld consoles (3DS, PSV) and role-playing games.

5.  **Statistical Hypothesis Testing:**
    *   **Hypothesis 1 (Xbox One vs. PC):** No significant difference in average user ratings (p-value = 0.549).
    *   **Hypothesis 2 (Action vs. Sports):** Significant difference exists in average ratings (p-value < 0.05).

## Results and Conclusions

*   **Dynamic market:** Platforms have predictable life cycles (6-10 years). It is crucial to stay updated with trends.
*   **Regional dominance:** Sony leads in NA and EU with home consoles; Nintendo has a greater presence in handhelds, especially in Japan.
*   **Profitability by genre:** Shooters and sports generate higher revenue per title, although action is more common.
*   **Success factors:** Reviews are not the only predictors; platform, genre, region, and marketing play a fundamental role.
*   **Recommended strategy:** Focus on leading platforms (PS4, XOne) and high-performing genres (shooters, sports) in Western markets; consider handhelds and role-playing games in Japan.

**How to Run the Project**

1.  Clone this repository to your local machine.
    ```bash
    git clone (https://github.com/ferchi4/Proyecto_spring_6)
    ```
    *(Note: Ensure you replace the URL with your actual repository URL).*

2.  Ensure you have the necessary dependencies installed:
    ```bash
    pip install pandas numpy matplotlib seaborn scipy jupyter
    ```

3.  Place the CSV files (`games.csv`) in the same directory as the notebook.

4.  Open and run the `proyecto10.ipynb` file in Jupyter Notebook.
    ```bash
    jupyter notebook proyecto10.ipynb
    ```

