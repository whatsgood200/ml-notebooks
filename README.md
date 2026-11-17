# ML notebooks

Early machine-learning projects from 2024, kept together in one place. Each folder holds one Jupyter notebook.

| Project | What it does | Approach | Result |
|---|---|---|---|
| [breast-cancer-neural-net](breast-cancer-neural-net/breast_cancer_neural_net.ipynb) | Classifies tumours as malignant or benign from 30 features | scikit-learn's breast cancer dataset, standard scaling, small Keras dense network | 97.4% test accuracy |
| [movie-recommender](movie-recommender/movie_recommender_tfidf.ipynb) | Suggests movies similar to one you type in | TF-IDF over genres, keywords, tagline, cast and director, then cosine similarity; fuzzy title match with `difflib` | Top similar titles |

## Run

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow jupyter
jupyter notebook
```

The movie recommender expects a `movies.csv` file in `movie-recommender/dataset/` (a TMDB movies export with `title`, `genres`, `keywords`, `tagline`, `cast` and `director` columns). It is not included in this repo.

## License

MIT
