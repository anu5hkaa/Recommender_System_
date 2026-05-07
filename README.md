#  Movie Recommendation System

A content-based movie recommendation system built using Machine Learning and NLP techniques. This project recommends movies similar to a user’s favorite movie by analyzing genres, keywords, cast, crew, and overview tags from the TMDB 5000 Movies Dataset. The system uses cosine similarity to find the most relevant movie recommendations.

---

## 🚀Features

- Recommend movies similar to a selected movie
- Uses content-based filtering
- NLP-based tag processing
- Cosine similarity for recommendation generation
- Data preprocessing and feature engineering
- Clean and efficient recommendation pipeline

---

## Dataset Used

- TMDB 5000 Movies Dataset
- TMDB 5000 Credits Dataset

The datasets contain:
- Movie title
- Genres
- Overview
- Keywords
- Cast
- Crew
- Ratings and popularity

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- NLP
- CountVectorizer
- Cosine Similarity
- Jupyter Notebook / Google Colab

---

##  Working Process

### 1. Data Collection
Loaded movie and credits datasets using Pandas.

### 2. Data Cleaning
- Removed null values
- Removed duplicate data
- Selected important columns only

### 3. Feature Engineering
Extracted:
- Genres
- Keywords
- Top 3 cast members
- Director name
- Movie overview

Combined all features into a single column called `tags`.

### 4. Text Processing
- Removed spaces from multi-word terms
- Converted text into tokens
- Applied vectorization using `CountVectorizer`

### 5. Similarity Calculation
Calculated cosine similarity between movie vectors.

### 6. Recommendation Function
Given a movie title, the system returns the top similar movies.

---

## Example

### Input:
```python

recommend("Avatar")
