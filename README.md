# CineMatch AI: Hybrid Movie Recommendation System

CineMatch AI is an end-to-end hybrid movie recommendation engine deployed as a responsive web application using Streamlit. It solves the challenge of digital content discovery by fusing Content-Based Filtering with Item-Item Collaborative Filtering, enhanced with live metadata from external entertainment APIs.

## 📌 Project Overview

With massive libraries available on modern streaming platforms, users face choice overload. CineMatch AI delivers precise recommendations by leveraging:

* **Content-Based Filtering:** Analyzes movie metadata (genres, keywords, cast, and director) using Natural Language Processing (NLP) and Cosine Similarity.

* **Collaborative Filtering:** Evaluates user interaction patterns from community ratings to uncover hidden behavioral similarities.

* **Hybrid Scoring Formula:**
  

  $$
  \text{Final Score} = 0.6 \times (\text{Content Score}) + 0.4 \times (\text{Collaborative Score})
  $$

The platform features automated live trending sections, rich movie details (synopsis, trailers, IMDb/Rotten Tomatoes ratings, cast & crew info), and user account/watchlist management.

## 📊 Datasets & Links

1. **TMDB 5000 Movie Dataset:**

   * Source: [TMDB 5000 Movie Metadata on Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?utm_source=gemini)

   * Usage: Content-based metadata extraction, tag synthesis, and text vectorization.

2. **MovieLens Latest Small Dataset:**

   * Source: [MovieLens Latest Datasets (GroupLens)](https://grouplens.org/datasets/movielens/?utm_source=gemini)

   * Usage: Calculating item-item collaborative similarity matrix based on user ratings.

## 🛠️ Technologies Used

* **Frontend / UI:** Streamlit (Custom CSS Dark Cinematic Theme, Session State Management)

* **Programming Language:** Python

* **Machine Learning & NLP:** Scikit-learn (CountVectorizer, Cosine Similarity), NumPy, Pandas

* **Data Serialization:** Pickle, AST

* **Database:** SQLite3 (Local Authentication & Watchlist Management)

* **External APIs:**

  * **TMDB API:** High-resolution posters, cast images, release metadata, and trailers

  * **OMDb API:** Aggregated IMDb and Rotten Tomatoes ratings

## 🚀 Setup & Run Instructions

### 1. Clone the Repository

```
git clone https://github.com/your-username/movie-recommendation-system.git
cd movie-recommendation-system

```

### 2. Create and Activate Virtual Environment

```
# Windows
python -m venv venv
venv\Scripts\activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate

```

### 3. Install Dependencies

```
pip install -r requirements.txt

```

### 4. Run the Streamlit Application

```
streamlit run app.py

```

## 🌟 Key Information & Features

* **Predictive Search Dropdown:** Select seamlessly from over 5,000 movie titles.

* **Hybrid Recommendations:** Top 5 similar titles displayed with dynamic similarity match percentages.

* **Rich Media View:** Direct access to YouTube trailers, director info, and cast showcase.

* **User Dashboard:** Built-in authentication with watchlist management.

* **Live Deployment:** [CineMatch AI Live App](https://movie-recommendation-system-eu8dufyzvpnc5tecnfxnct.streamlit.app/?utm_source=gemini)