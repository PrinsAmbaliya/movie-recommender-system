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


## ⚙️ How It Works
1. User enters:
   - Movie Title (from dropdown)
2. The request is processed by the Streamlit app.
3. The trained model recommends 5 similar movies with posters fetched from TMDB API.
4. Results are displayed on the webpage with movie titles and posters.

## 🚀 Installation & Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/PrinsAmbaliya/Movie_Recommender_System.git
   cd Movie_Recommender_System
2. **Create a Virtual Environment & Activate It**:
   ```bash
   python -m venv venv
   source venv/bin/activate    # Linux/Mac
   venv\Scripts\activate       # Windows
3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
4. **Run the Streamlit Server**:
   ```bash
   streamlit run app.py
5. **Open the App in Your Browser**:
   - Select a movie → get recommendations

## 📊 Model Training
-  Preprocessing: Merged datasets, extracted features (genres, keywords, cast, crew, overview),applied stemming with NLTK
-  Feature Engineering: Combined features into 'tags' column, vectorized with CountVectorizer (top 5000 features)
-  Model: Cosine Similarity matrix on vectorized tags
-  Saved: As movie_dict.pkl (processed data) and similarity.pkl (similarity matrix)

## 🖼 Screenshots
<img width="1908" height="1079" alt="image" src="https://github.com/user-attachments/assets/9aa20120-f7b4-46a9-8efb-d0cd5f5b6dfb" />

## 🔮 Future Improvements
-  Integrate advanced ML models (e.g., TF-IDF, Deep Learning embeddings)
-  Deploy live on Streamlit Sharing / Render
-  Expand dataset with TMDB API for real-time data
-  Enhance UI/UX with user ratings and hybrid filtering
-  Add more features like release year and popularity

##  👨‍💻 Author
Prins Ambaliya

GitHub: PrinsAmbaliya

LinkedIn: https://www.linkedin.com/in/prins-ambaliya-bb7546367
