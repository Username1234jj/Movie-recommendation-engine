# Movie Recommendation Engine

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Used-success.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.x-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Active-success.svg)

This project is a movie recommendation system that suggests movies to users based on their past ratings. It uses collaborative filtering to find similarities between users or items and then recommends the top movies that a user might like.

## Overview

The goal of this project is to build a simple recommendation engine that can analyze user-movie rating data and predict which movies a user would enjoy. It demonstrates the basic concept behind systems like Netflix or IMDb recommendations.

## Features

- Reads user ratings and movie data
- Creates a user-movie matrix
- Uses collaborative filtering (item-based or user-based)
- Calculates similarities between users or movies
- Recommends top movies for a selected user
- Easy to run and understand

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook (for experiments)

## Dataset

You can use any movie rating dataset.
For example, the **MovieLens dataset** from https://grouplens.org/datasets/movielens/.
It should contain at least three columns:
- userId
- movieId
- rating

Optionally, you can include a `movies.csv` file with:
- movieId
- title

## Project Structure

```
Movie-recommendation-engine/
│
├── movie_recommender.py
├── Movie_Recommendation_Engine_Collaborative_Filter.ipynb
├── data/
│   ├── ratings.csv
│   └── movies.csv
├── requirements.txt
└── README.md
```

## Installation and Setup

1. Clone the repository
   ```
   git clone https://github.com/Username1234jj/Movie-recommendation-engine.git
   cd Movie-recommendation-engine
   ```
2. Install dependencies
   ```
   pip install -r requirements.txt
   ```
3. Make sure your data files (`ratings.csv`, `movies.csv`) are in the `data/` folder.

## How to Run

You can either run the Python script or open the Jupyter notebook.

**To run the script:**
```
python movie_recommender.py
```

**To use the notebook:**
```
jupyter notebook Movie_Recommendation_Engine_Collaborative_Filter.ipynb
```

Then follow the steps inside the notebook to train the model and get recommendations.

## How It Works

1. Load the dataset (ratings and movies).
2. Build a user-movie rating matrix.
3. Compute similarity between users or items.
4. Predict ratings for movies the user hasn't seen yet.
5. Sort the results and recommend the top-rated movies.

## Example Output

For a sample user, the engine will show something like:
```
 movieId   score   title
     1     4.85    Toy Story (1995)
     2     4.73    Jumanji (1995)
     3     4.62    Grumpier Old Men (1995)
```

## Future Improvements

- Add a web interface using Flask or Streamlit
- Try deep learning methods for recommendations
- Add evaluation metrics (RMSE, precision, recall)
- Include content-based filtering for hybrid recommendations

## Acknowledgements

- MovieLens dataset by GroupLens Research
- Inspiration from collaborative filtering tutorials and open-source projects

## License

This project is open-source and free to use for educational purposes.
