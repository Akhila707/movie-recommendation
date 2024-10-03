Movie Recommendation System
“Ever had Netflix ask, ‘Are you still watching?’ Well, now you’ll never want to stop!”

1. Overview
This project is a movie recommendation system that uses machine learning techniques to suggest movies similar to your favorites. It leverages cosine similarity between movies based on features like genre, cast, and keywords.

2. How It Works
Input: You provide the name of a movie you like.
Output: A list of recommended movies based on similarities in features like genre, keywords, cast, tagline, and director.
3. Key Features
TF-IDF Vectorizer:
Converts text features (genres, keywords, tagline, etc.) from the movie dataset into numerical vectors using the TfidfVectorizer.

Cosine Similarity:
Calculates the cosine similarity between movie vectors to recommend movies that are closest in terms of features.

Difflib:
Handles fuzzy matching to ensure the system can recommend even if the movie title input is not exact.

4. Libraries Used
numpy:
For numerical operations.

pandas:
For data manipulation and analysis.

difflib:
To find close matches of movie names.

sklearn:
Used for TF-IDF vectorization and cosine similarity calculations.

5. Key Methods
TF-IDF Vectorization:
Converts text data to numerical form, which is essential for similarity calculations.

Cosine Similarity:
Measures the similarity between the feature vectors of movies, used to rank and recommend similar movies.

Data Handling:

Replacing null values in the dataset to avoid errors during vectorization.
Combining multiple features (genre, cast, keywords, tagline, director) into a single string for each movie to create richer vectors for comparison.
Performance:
The system ranks movies based on similarity and suggests the top similar movies for you to enjoy.
