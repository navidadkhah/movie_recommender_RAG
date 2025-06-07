# Movie & Series Recommendation System
This repository implements a Retrieval-Augmented Generation (RAG) pipeline for suggesting movies and series based on user queries and a custom database built using TMDB APIs. Users can get personalized recommendations by entering descriptions like:

"I want a movie like Interstellar but a little funnier"

# Features
- Automated Data Collection: Collects movies and series data from the TMDB API.

- Custom Database Creation: Stores data in a CSV file, then loads it into ChromaDB.

- Natural Language Recommendations: Users can describe what kind of movie/series they want in plain English.

# How It Works
1- Data Collection:

Use data_collector.ipynb to fetch movies and series metadata from TMDB, storing results in a CSV file.

2- Database Creation:

Run Creating_DB.ipynb to initialize ChromaDB and import your CSV data.

3- User Query:

Users can enter natural language queries (e.g., "I want a movie like Interstellar but a little funnier"), and the system suggests the closest matches based on embeddings and similarity search.


# Usage Example

- Example user query:
user_input = "I want a movie like Interstellar but a little funnier"

- The system returns a list of recommendations based on similarity.
Notes
Make sure to update embeddings whenever new data is added.






