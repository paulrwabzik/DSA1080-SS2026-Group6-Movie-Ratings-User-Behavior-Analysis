# DSA1080-SS2026-Group6-Movie-Ratings-User-Behavior-Analysis

# Dataset source link:[(https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset)]

# Number of rows: 45467 rows

# Participants 

* 1.Rwabajungu Paul-676390
* 2.Pearl Osong - 676306
* 3.Staicy Kimberly-677494
* 4.Trevor Ndungi-675561
---
# Tools used
* Language: Python 3.10
* Libraries: Pandas (Data Wrangling), NumPy (Mathematical Transformations), Scikit-Learn (Machine Learning), Matplotlib (Visualization).
* Version Control: Git/GitHub.
* Environment: Jupyter Notebook.
---
# The Regrssion Analysis
The regressiona analysis was entirely crucial for understanding user behavior; for this reason Artificial Intelligence was used to perfrom a Random Forest Regressor analysis. Artificial Intelligence was also used to perfrom the **Hot encoding** used to separate the genres from a dictionary into separate binary columns.

Our group opted out of a simple linear regression because it was unsuitable for this dataset due to the non-linear nature of features like budget and popularity. 
The dataset also contains repeated measures (multiple ratings per user).

The Random Forest Regressor was chosen instead because it effectively captures complex relationaships  between features and handles categorical genre data without requiring strict linearity.

# Findings
The regression found that the top factors that contribute most towards ratings are;
- **user_mean_rating**:Showing that the best way to tell how someone will rate a movie is to see how they have rated in the past.
- **popularity**:That users are influenced to like something based on how popular it is at the time.
- **revenue_log**:The more revenue a movie makes the more like watched it is, positively impacting its ratings.
- **budget_log**:The more money is pured into a movie, the better the quality, the better the rartings.
- **runtime**-Movies that are too long or too short often times get lower rating becuase of human intest and attention span affecting its rating.
- **vote_count**: This is the number of global votes  a certain movie has using the TMDB  database showing that higher global ratings  mean a better rating.
- **vote_average**:A higher vote average means a the more liked the movie is globally the better ratings its going to receive.

