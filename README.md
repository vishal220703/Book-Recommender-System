# 📚 Book Recommendation System

This project is a **Flask web application** that recommends books based on user input. It leverages collaborative filtering to suggest similar books using precomputed similarity scores.

## 🔍 Features

- View popular books with average ratings and number of votes
- Get personalized book recommendations based on your favorite book
- Clean and simple UI built with HTML templates and Flask backend

## 🚀 How It Works

- Loads precomputed data (`popular.pkl`, `pt.pkl`, `books.pkl`, `similarity_scores.pkl`)
- On the homepage (`/`), displays a list of most popular books
- On the `/recommend` page, users can enter a book title to get 4 similar recommendations

## 🧠 Recommendation Logic

- Uses cosine similarity on pivot table (`pt`) to find similar books
- Recommendations are extracted using similarity scores
- Book details like author and cover image are fetched from the `books` dataset

## 🛠️ Installation

1. Clone the repository
2. Ensure you have `Flask`, `numpy`, and `pickle` installed
3. Place the required `.pkl` files in the root directory
4. Run the app:

```bash
python app.py
```
