# 🎬 Movie Recommendation System

This project implements a basic movie recommendation system using a combination of movie metadata and user ratings. It utilizes machine learning models to classify movies as "recommended" or "not recommended" based on user ratings and genre information.

## 📁 Dataset

The system uses the [MovieLens](https://grouplens.org/datasets/movielens/) dataset, which includes:

- `movies.csv`: Contains movie IDs, titles, and genres.
- `ratings.csv`: Contains user ratings of movies.

## 🛠️ Features

- Merges rating and movie metadata.
- Extracts and one-hot encodes genre information.
- Labels ratings as recommended (1 if rating ≥ 4, else 0).
- Trains classification models to predict user preferences.

## 🧪 Machine Learning Models

The following models are used to classify recommendations:

- Random Forest Classifier
- Logistic Regression

## 🧩 Libraries Used

- `pandas`, `numpy`: Data manipulation
- `sklearn`: Machine learning and preprocessing

## 🔍 How it Works

1. **Data Preprocessing**:
   - Genres are split and one-hot encoded using `MultiLabelBinarizer`.
   - Labels are created based on whether a rating is ≥ 4.

2. **Model Training**:
   - The genre features are used to predict whether a user would recommend the movie.
   - Models are evaluated using accuracy and classification report.

## 📈 Evaluation Metrics

- Accuracy Score
- Classification Report (Precision, Recall, F1-score)

## 🚀 How to Run

1. Download the MovieLens dataset.
2. Place `movies.csv` and `ratings.csv` in your working directory.
3. Open the notebook and run all cells.

## ✅ Future Improvements

- Use collaborative filtering or hybrid recommendation methods.
- Include user-based and item-based features.
- Incorporate deep learning methods (e.g., autoencoders).

## 📜 License

This project is for educational purposes only. Refer to the MovieLens license for dataset usage.
