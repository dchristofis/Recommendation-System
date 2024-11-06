# Recommendation-System
Netflix Movies - -Bert - Transformer - word2vec 

This project is a movie recommendation system for Netflix users, built using content based filtering. The system recommends movies based on:

Award-Winning Movies and Preferences: Combining highly acclaimed (awarded) movies with the user's preferences to offer recommendations.
Genre-Based Recommendations: Recommending movies from the same genre based on what the user has watched previously.
Specific Movie Ratings: If the user highly rates (e.g., 5 stars) a movie, the system recommends similar movies based on genre, year, and popularity.
The recommendation system integrates both collaborative filtering (leveraging user preferences and behavior) and content-based filtering (utilizing movie metadata such as genre, year, etc.).

## Key Features
Word2Vec for Movie Embeddings: Using the Word2Vec model to create movie embeddings based on genre, year, and other metadata. These embeddings help group similar movies together for better recommendations.
Bert & Transformers
Content-Based Filtering: Recommends movies that share features like genre, release year, or popularity with those highly rated by the user.

## Workflow
Data Preprocessing: Clean and preprocess the data. This involves handling missing values, normalizing user ratings, and encoding movie metadata (e.g., genre and year).

Movie Embeddings using Word2Vec: Word2Vec is applied to learn vector representations of movies. Each movie is treated like a word in a sentence, with features like genre and year helping group similar movies together.

Content-Based Filtering: Recommends movies based on their similarity in metadata (genre, year, etc.) to the movies the user has highly rated.

Hybrid Model: The final recommendation combines the results of collaborative filtering and content-based filtering for a comprehensive recommendation experience.


## Usage
Rating-Based Recommendations: The system will recommend movies similar to those highly rated by the user (e.g., 5-star ratings).

Genre-Based Recommendations: If the user enjoys a specific genre, the system will suggest other popular movies within that genre.

Award-Winning Recommendations: The system can prioritize recommending highly awarded movies that align with the user's preferences.

## Future Enhancements
User Interactions: History of the user's viewing activity, ratings provided by the user on different titles, and their interaction patterns.
Collaborative Filtering: Leveraging user-to-user similarities based on viewing history, ratings, and other interactions, enabling personalized recommendations by identifying users with similar preferences.
Incorporating real-time user feedback to improve recommendations.
Collaborative Filtering: Uses user rating data to identify similar users and recommend movies that users with similar tastes have enjoyed. We implement matrix factorization (such as SVD or ALS) to handle large user-item matrices.
Hybrid Approach: Combines both collaborative filtering (user-to-user interactions) and content-based filtering (movie metadata like genre and year) for more accurate recommendations.
Adding user-defined filters (e.g., only recommending movies from certain years or avoiding specific genres).
Enhancing the award-based weighting to emphasize critically acclaimed movies.

## Conclusion
This recommendation system uses movie metadata to generate personalized, accurate movie recommendations. The combination of Word2Vec, embeddings and content-based filtering provides a powerful recommendation tool for Netflix-style applications.