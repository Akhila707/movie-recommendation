Movie Recommendation System 🍿🎬
“Ever had Netflix ask, ‘Are you still watching?’ Well, now you’ll never want to stop!”

1.Overview
This project is a movie recommendation system built using machine learning techniques to suggest movies similar to your favorites. It uses the cosine similarity between movies based on various features like genre, cast, and keywords.

2.How It Works:
--Input: You provide the name of a movie you like.
--Output: A list of recommended movies based on similarities in features like genre, keywords, cast, tagline, and director.
3.Key Features:
--TF-IDF Vectorizer: Text features from the movie dataset (like genres, keywords, tagline, etc.) are converted into numerical vectors using the TfidfVectorizer.
--Cosine Similarity: The model calculates the cosine similarity between the movie vectors, allowing it to recommend movies that are closest in terms of these features.
--Difflib: This is used to handle fuzzy matching, ensuring the system can recommend even if the movie title input isn’t exact.

4.Libraries Used:
---numpy: For numerical operations.
---pandas: For data manipulation and analysis.
---difflib: To find close matches of movie names.
---sklearn: Specifically used for TF-IDF vectorization and cosine similarity calculations.

5.Key Methods:
--TF-IDF Vectorization: Converts text data to numerical form, which is essential for similarity calculations.
--Cosine Similarity: Measures the similarity between the feature vectors of movies, used to rank and recommend movies.
--Data Handling:Replacing null values in the dataset to avoid errors during vectorization. Combining multiple features into a single string for each movie to create richer vectors for comparison.
--Performance:The system ranks movies based on similarity and suggests the top similar movies for you to enjoy.
