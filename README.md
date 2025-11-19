# Book Recommender (SVD)

Book Recommender is a Python project that builds a personalized book recommendation system using Singular Value Decomposition (SVD). The project was developed as part of a data processing and machine learning course, following the CRISP-DM process model. The goal is to explore how collaborative filtering can be applied to a real-world dataset to predict user ratings and suggest new books.

---

## Features

- **SVD-Based Collaborative Filtering**: Learns latent user and item factors from rating data using matrix factorization.
- **Data Exploration & Visualization**: Rating distributions, user activity, sparsity levels, and error histograms.
- **Top-N Recommendation Function**:  Generates personalized book suggestions for any user.
- **Custom User Profiles**:  Supports adding external rating profiles to test personalized recommendations.

---

## Technical Specifications

* **Language:** Python
* **Libraries:** Surprise, Pandas, NumPy, Matplotlib
* **Model:** SVD (matrix factorization)
* **Data:**
   * `ratings.csv` – user/book rating pairs
   * `books_enriched.csv` – metadata (title, author, genre, etc.)
* **Environment:** Jupyter Notebook

---

## Getting Started

### Prerequisites

* Python 3.10+
* Jupyter Notebook
* Required libraries installed:
```bash
  pip install scikit-surprise pandas numpy matplotlib jupyter
```

### Setup

1. Clone the Repository
```bash
   git clone https://github.com/Jonnerop/Book-Recommender.git
   cd Book-Recommender
```

2. Open the notebook:
```bash
   jupyter notebook
```

3. Run the main analysis file: `book_recommender.ipynb`

---

## Usage

1. Load datasets (`ratings.csv` & `books_enriched.csv`)
2. (Optional) Add a new user with custom ratings
3. Train or load the SVD model
4. Generate recommendations:
```python
   get_top_n(user_id, n=10)
```
5. View book titles and predicted scores for any user.

---

## Future Enhancements

* Hyperparameter tuning for improved accuracy
* Hybrid model combining metadata with collaborative filtering
* Web-based frontend for interactive recommendations
* Cold-start handling using popularity-based suggestions
