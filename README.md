# 50.045 Information Retrieval Project
Anime Recommendation Engine

Anime is a popular style of Japanese film and television animation. It has a huge plethora of shows and episodes for one to choose from. This makes it all the more harder for one to find a specific anime or to find new animes to watch after completing one. In this project, we harnessed information retrieval to allow one to search for an anime faster as well as ones related to it using text queries.

# Raw Dataset

Anime Recommendation Database 2020 (Kaggle): https://www.kaggle.com/code/karthikayyala/anime-reccomendation/data
Recommendation data from 325,772 users and 17,562 animes
1. anime.csv [17562, 35]
2. anime_with_synopsis.csv [16214, 35]
3. animelist.csv [10922747, 5]
4. rating_complete.csv [57633278, 3]
5. watching_status.csv [2, 5]

# Approaches
1. Best Match 25 (BM25)
2. Vector Space Model (VSM)
3. Latent Semantic Analysis (LSA)

# Evaluation Dataset
1. Randomly extracted 50 rows from raw data as test set.
2. Manually crafted 10 test queries.
3. Manually labelled relevance score for each data point and query.

# Evaluation Metrics
1. Mean Average Precision (MAP)
2. Mean Normalized Discounted Cumulative Gain (nDCG)
3. Mean Reciprocal Rank (MRR)
4. Latency


# Final Takeaways
1. Lack of evaluation dataset.
  Manually crafted queries and labelled data might be biased
  Too small a test set, not representative
2. LSA was expected to be best performing - possibly need to make a more extensive evaluation dataset
3. BM25 can be improved by implementing variations which assign weights to different attributes (Synopsis vs Name vs Genres etc)
4. Query expansion with synonyms for recommendation
  Can use user review scores to rank results too


