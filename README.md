# Movie Recommender System

Welcome to the Movie Recommender System, a simple recommendation engine built for movie enthusiasts. This project is a part of my journey into machine learning, and it suggests movies based on their similarity to a user-selected movie.

## Demo
Check out the live demo of the Movie Recommender System [here](https://tkm-movie-recommender.streamlit.app/).

## Overview

### Data Source
The movie database used for this project is sourced from [TMDB (The Movie Database)](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata/), comprising information on 5000 movies.

### Data Processing
The data underwent refinement, utilizing features such as title, cast, crew, overview, keywords, and genres to create tags for each movie. These tags were then vectorized using the `CountVectorizer` from the scikit-learn library.

### Similarity Calculation
Cosine similarity was employed, utilizing the `cosine_similarity` function from `sklearn.metrics.pairwise`, to calculate the similarity between movies based on their tag vectors. This similarity metric aids in identifying movies that share common characteristics.

### Word Stemming
To identify different forms of similar words, the project makes use of the `PorterStemmer` from the `nltk.stem.porter` module.

## Installation and Usage

```bash
# Clone the repository:
git clone https://github.com/your-username/movie-recommender.git

# Install the required dependencies:
pip install -r requirements.txt

# Run the app:
streamlit run app.py
```

## Credits and Acknowledgements
- [TMDB 5000 Movie Dataset](https://www.kaggle.com/tmdb/tmdb-movie-metadata) by [TMDB](https://www.themoviedb.org/) on Kaggle
- [Movie Recommender System](https://www.youtube.com/watch?v=1xtrIEwY_zY&list=PLKnIA16_RmvY5eP91BGPa0vXUYmIdtfPQ) by [CampusX](https://www.youtube.com/@campusx-official) on YouTube
- [Streamlit](https://www.streamlit.io/) for the web app framework
- [scikit-learn](https://scikit-learn.org/stable/) for the machine learning library
- [NLTK](https://www.nltk.org/) for the natural language processing library
