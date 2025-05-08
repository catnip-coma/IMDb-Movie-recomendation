# IMDb Movie Recommendation System
A hybrid Movie Recommendation System using K-Means clustering and content-based filtering (TF-IDF & cosine similarity) to suggest movies similar to a given input.

## Overview
Finding a great movie to watch can be overwhelming. This project builds a smart recommendation system that suggests movies based on their genres, content, and clustering.

## Features
✔️ Hybrid Recommendation Approach – Uses clustering and content similarity for better suggestions. 
✔️ K-Means Clustering – Groups movies based on feature similarities. 
✔️ TF-IDF & Cosine Similarity – Improves accuracy by analyzing movie descriptions. 
✔️ Scalable Model – Works with large datasets efficiently.

## Dataset
The dataset is sourced from the IMDb Top 5000 Movies, containing essential movie metadata such as: 🔹 Title (primaryTitle) 🔹 Year of Release (startYear) 🔹 Ratings & Votes (averageRating, numVotes) 🔹 Genres (genre_list) 🔹 Crew Information (directors, writers)

## Methodology
### 1️⃣ Data Preprocessing

Extracted genres & crew information

Normalized numerical values using MinMaxScaler

Prepared text features for TF-IDF vectorization

### 2️⃣ K-Means Clustering

Movies grouped into clusters based on features

Cluster assignment used for filtering recommendations

### 3️⃣ Content-Based Filtering

TF-IDF used to vectorize text-based metadata

Cosine similarity computed for finding similar movies

## Installation & Usage
### Setup
1. Install dependencies:
```python
pip install pandas numpy sklearn matplotlib seaborn
```
2. Run Jupyter Notebook or Python script.

## Usage
```python
# Example: Recommend movies similar to "Ice Age"
recommended_movies_df = recommend_movies("Ice Age", n=5)
print(recommended_movies_df)
```
## Results
The system provides personalized movie recommendations by combining clustering (grouping similar movies) and content analysis (plot + genre matching).

## Outcomes and Learnings
- Gained hands-on experience with unsupervised learning algorithms
- Practiced feature extraction, text vectorization, and similarity computations
- Understood the pipeline of building a real-world recommendation engine
- Applied industry tools like Scikit-learn and CountVectorizer in a practical scenario

## Future Improvements
🔹 Include actor-based filtering 
🔹 Enhance recommendations using collaborative filtering 
🔹 Use deep learning for better accuracy

## Acknowledgment
This project was completed as part of the AICTE Edunet Internship, and is inspired by the open-source work of @therohitshelar97.
