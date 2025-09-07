# 🎥 Movie Recommender System

A **Machine Learning + Streamlit Web App** to recommend similar movies based on title, using content-based filtering with genres, keywords, cast, crew, and overview from the TMDB dataset.

## 📌 Project Overview
- **Dataset**: TMDB 5000 Movie Dataset (`tmdb_5000_movies.csv`, `tmdb_5000_credits.csv`)
- **Model**: Cosine Similarity (on vectorized text features with CountVectorizer and stemming)
- **Backend**: Python Streamlit API (`app.py`)
- **Frontend**: Streamlit UI (integrated in `app.py` with poster fetching from TMDB API)
- **Deployment Ready**: Can be hosted on Streamlit Sharing / Heroku / Render / AWS

## 🗂 Project Structure

```
├── model/
│   ├── movie_dict.pkl                      # Pickled DataFrame of processed movie data
│   ├── similarity.pkl                      # Pickled cosine similarity matrix
│
├── data/
│   ├── tmdb_5000_movies.csv                # Raw movie details dataset
│   ├── tmdb_5000_credits.csv               # Raw credits dataset
│
├── notebooks/
│   └── movie-recommender-system.ipynb      # Jupyter notebook for EDA & model training
│
├── app.py                                  # Streamlit server and UI
├── requirements.txt                        # Dependencies
└── README.md                               # Project Documentation
```

