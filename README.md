# 🎬 Movie Recommendation System

This project is a **content-based recommendation system** built using the TMDB 5000 Movies Dataset.  
It suggests movies similar to a given movie based on **overview, genres, keywords, cast, and crew**.

---

## 📌 Project Overview
The system analyzes movie descriptions and metadata to find similarities between films.  
By combining text features into a single representation and applying **cosine similarity**, the model can recommend the top 5 most relevant movies for any chosen title.

Example:  
If you search for **"Avatar"**, the system might recommend:  
- Titan A.E.  
- Independence Day  
- Ender’s Game  
- Small Soldiers  
- Aliens vs Predator: Requiem  

---

## ⚙️ How It Works
1. Load and merge datasets (`tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`).  
2. Extract and clean useful features: **overview, genres, keywords, cast, crew**.  
3. Combine these into a single column called **tags**.  
4. Convert text data into numerical vectors using **CountVectorizer**.  
5. Calculate similarity between all movies using **cosine similarity**.  
6. Build a `recommend()` function that returns the top 5 similar movies.

---

## 🛠️ Technologies Used
- Python  
- Pandas, NumPy  
- Scikit-learn (CountVectorizer, cosine_similarity)  

---
