# 🎵 Music Recommendation System

A **content-based music recommender system** that suggests songs similar to your favorite track using audio features like energy, mood, tempo, and more.

Built using Python, Pandas, and scikit-learn, this system is optimized to run efficiently even on large datasets (130k+ songs) without memory errors.

---

## 📌 Features

- Recommend songs similar to any given track
- Uses Spotify audio features like:
  - Acousticness, Danceability, Energy, Valence, Tempo, etc.
- Cosine similarity for finding closeness between songs
- Scaled features for better accuracy
- Memory-efficient using `NearestNeighbors` (no full similarity matrix)
- Displays results directly in Jupyter Notebook

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/music-recommender.git
   cd music-recommender
   ```

2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook:
   ```bash
   jupyter notebook music_recommender.ipynb
   ```

4. Enter any song name when prompted:
   ```bash
   🎵 Enter a song name: believer
   ```

5. You’ll get the top 5 similar songs with similarity scores.

---
   
## 📊 Example Output
```
| track\_name        | artist\_name              | similarity\_score |
| ------------------ | ------------------------- | ----------------- |
| Shoot My Shot      | Jøhansen                  | 0.96              |
| Oh Meri Sajiniyare | Dr. Vaikkom Vijayalakshmi | 0.96              |
| South of Somewhere | Southern Justis           | 0.96              |
| Wake up the Saints | Levi Riggs                | 0.95              |
| Safer              | Noise Killers             | 0.95              |
```

---

## 💡 How it Works

- Load a dataset of songs with audio features

- Clean and standardize the data

- Normalize audio features with StandardScaler

- Use NearestNeighbors with cosine distance to find similar songs

---

## 📦 Requirements

```nginx
pandas
scikit-learn
```

