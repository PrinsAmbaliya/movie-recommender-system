<<<<<<< HEAD
# Movie Recommender System

![Project Icon](./icon.png)

Welcome to the **Movie Recommender System**, a content-based movie recommendation engine developed by [Prins Ambaliya](https://github.com/PrinsAmbaliya). This project leverages the TMDB 5000 Movie Dataset to suggest the top 5 movies similar to a given title, based on features such as genres, keywords, cast, crew, and plot overviews. Built with Python and modern machine learning techniques, this system is an excellent example of natural language processing (NLP) and cosine similarity applications.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Files in the Repository](#files-in-the-repository)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

## Project Overview
The Movie Recommender System is designed to provide personalized movie recommendations by analyzing movie metadata. It preprocesses text data using NLP techniques, converts it into numerical vectors, and computes similarity scores to rank relevant movies. This project is ideal for learning data preprocessing, feature engineering, and recommendation system development.

## Dataset
- **Source**: [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) from Kaggle.
- **Files**:
  - `tmdb_5000_movies.csv`: Contains movie details (title, genres, keywords, overview, etc.).
  - `tmdb_5000_credits.csv`: Includes cast and crew information.
- **Size**: Approximately 5,000 movies.
- **Note**: Due to GitHub's file size limits, the CSV files are not included in this repository. Users must download them from Kaggle and place them in the project root directory.

## Features
- Merges and preprocesses TMDB datasets for analysis.
- Applies stemming to normalize text data.
- Utilizes CountVectorizer for feature extraction.
- Computes cosine similarity to identify similar movies.
- Provides a simple function to recommend the top 5 similar movies.

## Technologies Used
- **Programming Language**: Python 3.12.7
- **Libraries**:
  - `pandas`: Data manipulation and analysis.
  - `numpy`: Numerical computations.
  - `nltk`: Natural language processing (Porter Stemmer).
  - `scikit-learn`: Machine learning (CountVectorizer, cosine similarity).
  - `ast`: Parsing JSON-like strings.
  - `pickle`: Serialization for model persistence.
- **Development Tools**: Jupyter Notebook, Visual Studio Code.

## Installation
To set up the project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/PrinsAmbaliya/Movie_Recommender_System.git
   cd Movie_Recommender_System
=======
# Movie_Recommeder_System
>>>>>>> 1e17030 (Initial commit)
