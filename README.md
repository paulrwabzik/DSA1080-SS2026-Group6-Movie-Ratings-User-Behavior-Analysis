# DSA1080-SS2026-Group6-Movie-Ratings-User-Behavior-Analysis

## Dataset source link:[(https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset)]

-Number of rows: 45467 rows

## Participants 

- 1.Rwabajungu Paul-676390
- 2.Pearl Osong - 676306
- 3.Staicy Kimberly-677494
- 4.Trevor Ndungi-675561
- 5.Joy Migwi - 676291
- Peris Kasyoki-677135
---
## Data Dictionary
- userId- The unique identifier for every user who rated a movie.
- movieId- The identifier for every movie rarted.
- rating- Score given to a movie by a user on the scale of 0-5 with increments of 0.5.
- timestamp- the time the rating was made.
- adult- Whether the movie in question is the movie is meant specificaly for adult audiences.
- budget- The production expense of the movie in United States dollars($).
- genres-The category of film the movie falls into.
- popularity- A trend metric from TMBD(global movie database) indicating how much excitememt a movie has to the larger public.
- revenue- The capital made from the movie in United States dollars($).
- runtime-How long the movie is in minutes.
- vote_average-The average of the TMBD votes.
- vote_count-The totla number of user rating submitted globally for that movie.
- original language- The language the movie was originally produced in.
- bugdet_log- The production budget transormed using a log scale to handle extreme outliers.
- revenue_log-The capital grossed adjusted using a log scale to handle extremem outliers.
- user_mean_rating- This is the average rating given by a specific user across all movies watched. 
- user_rating_count- The sum of movies rated by a specific user
- release_date- The date the movie was released to the public
  
## Tools used
- Language: Python 3.10
- Libraries: Pandas (Data Wrangling), NumPy (Mathematical Transformations), Scikit-Learn (Machine Learning), Matplotlib (Visualization).
- Version Control: Git/GitHub.
- Environment: Jupyter Notebook.
---
# The Regression Analysis
- The regressiona analysis was entirely crucial for understanding user behavior; for this reason Artificial Intelligence was used to perfrom a Random Forest Regressor analysis. Artificial Intelligence was also used to perfrom the **Hot encoding** used to separate the genres from a dictionary into separate binary columns.
- Our group opted out of a simple linear regression because it was unsuitable for this dataset due to the non-linear nature of features like budget and popularity. 
- The dataset also contains repeated measures (multiple ratings per user).
- The Random Forest Regressor was chosen instead because it effectively captures complex relationaships  between features and handles categorical genre data without requiring strict linearity.
---
# Key Findings
- The "Blockbuster" Financial Model: Global net income is heavily "top-heavy." A small percentage of high-budget franchises (e.g., Lord of the Rings, Harry Potter) accounts for the majority of the $2.52 Trillion profit. This proves that existing Intellectual Property (IP) is the strongest predictor of financial returns.
- Popularity vs. Cultural Longevity: There is a difference between "Hype" and "Legacy." While Pulp Fiction has a high popularity score, The Dark Knight leads in total votes. This indicates that superhero and action genres maintain active fan base years after release.
- The Operational "Sweet Spot": The average runtime of 109 minutes (1hour 49minutes) highlights an industry standard. This duration is the optimal balance between audience retention and maximizing the number of daily theatre screenings.

##The Regression
The regression found that the top factors that contribute most towards ratings are;
- **user_mean_rating**:Showing that the best way to tell how someone will rate a movie is to see how they have rated in the past.
- **popularity**:That users are influenced to like something based on how popular it is at the time.
- **revenue_log**:The more revenue a movie makes the more like watched it is, positively impacting its ratings.
- **budget_log**:The more money is pured into a movie, the better the quality, the better the ratings.
- **runtime**-Movies that are too long or too short often times get lower rating becuase of human intest and attention span affecting its rating.
- **vote_count**: This is the number of global votes  a certain movie has using the TMDB  database showing that higher global ratings  mean a better rating.
- **vote_average**:A higher vote average means a the more liked the movie is globally the better ratings its going to receive.

##


