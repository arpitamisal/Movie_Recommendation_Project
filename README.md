🎬 Movie Recommendation System (Cosine Similarity Based)

This project is a simple movie recommender system built using item-based collaborative filtering with cosine similarity. It suggests movies similar to a given movie based on user rating patterns—no machine learning models used.

🚀 Project Overview

    Goal: Recommend movies that are similar to a selected movie

    Approach: Item-based collaborative filtering using cosine similarity

    Dataset: movies.csv (https://www.kaggle.com/datasets/harshshinde8/movies-csv)

    Tech stack: Python, pandas, NumPy, Seaborn, Matplotlib

🧬 Data Description

    movies.csv: Contains movieId, title, and genres

Merged both datasets and pivoted to form a user-movie matrix used for similarity calculations.
🧹 Preprocessing Steps

    Read and cleaned the dataset

    Created a pivot table: rows = users, columns = movies, values = ratings

    Replaced missing values with empty string

    Computed pairwise cosine similarity between movie columns

🤖 Recommendation Logic

    Input a movie title

    Extract its column vector from the user-movie matrix

    Calculate cosine similarity with all other movies

    Return the top N most similar movies (excluding the input)
    
📊 Visualization

    Distribution of movie ratings

    Popular movies by number of ratings

    Heatmap showing similarity between selected movies

💻 How to Run

    Clone this repo

    Install dependencies:

pip install -r requirements.txt

    Run the notebook:

jupyter notebook MovieRecommendation.ipynb

📽️ Sample Output

    Input Movie: Forrest Gump 
    Top Recommendations:

        The Shawshank Redemption 

        Apollo 13 

        Philadelphia 

        Rain Man 

🧠 Limitations

    Only recommends based on rating patterns, not content or genre

    No ML model or deep personalization for individual users
