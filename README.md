# Movie Recommendation System
This project presents a Content-Based Movie Recommendation System that suggests similar movies to users based on various attributes such as genres, keywords, cast, and crew using Natural Language Processing (NLP) and machine learning techniques.
---
##  Objective
- Recommend similar movies based on metadata.
- Enhance user experience on entertainment platforms.
- Reduce decision fatigue through intelligent suggestions.

---
##  Dataset

- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv
-  These datasets were manually downloaded from Kaggle and are stored locally on the desktop

  ---
  ##  Technologies Used
  - Python
- Pandas, NumPy
- NLTK
- Scikit-learn (CountVectorizer, Cosine Similarity)
- Jupyter Notebook

---
##  How It Works
1. **Data Merging** – Combines `movies` and `credits` datasets on the movie title.
2. **Feature Extraction** – Pulls out relevant data like overview, genres, cast, crew.
3. **Text Preprocessing** – Cleans and combines all text data into a single feature column.
4. **Vectorization** – Converts text into numerical vectors using `CountVectorizer`.
5. **Similarity Calculation** – Uses `cosine_similarity` to compute how similar movies are.
6. **Recommendation** – Recommends top 5 movies similar to the one entered.

---
##  How to Run the Project

1. Clone this repository or download the `.ipynb` file.
2. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn nltk

3. Place the tmdb_5000_movies.csv and tmdb_5000_credits.csv files in the same folder.
4. Run the Jupyter Notebook.

---

5. Use the following function to get recommendations:
   ```python
   recommend('Spider-Man 2')

---
## Example Output
 Top 5 recommendations for 'Spider-Man 2':
- Spider-Man 2
- Due Date
- I Love You, Man
- The Basket
- Avatar
