# Movies Recommender System

A content-based movie recommender system built during my internship at Ethical Edufabrica Pvt. Ltd.  
The system suggests similar movies based on plot descriptions and metadata features using TF-IDF and cosine similarity.

---

## 📂 Dataset

- Source: Kaggle  
- Records: **10,000 movies**  
- Features used: index, title, overview, vote average, vote count and popularity 

---

## 🧠 Approach

- Combined metadata fields into a single text representation for each movie
- Transformed text using `TfidfVectorizer`
- Computed cosine similarity to find most similar movies to a given input
- Integrated fuzzy matching (`difflib.get_close_matches`) to accept minor typos or variations in movie titles

---

## 🛠 Tools & Libraries

- Python · pandas · NumPy · scikit-learn · difflib · Jupyter Notebook

---

## ✅ Output

- Console-based input: user types a movie title
- Returns top 10 similar movies based on cosine similarity scores
- Supports partial input / spelling variations

---

## 📘 Usage

Run the notebook in Jupyter and enter a movie name when prompted:
```python
recommend("Inception")
