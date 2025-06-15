# Recommender-System-Personalized-Movie-Recommendations

To develop a personalized movie recommendation system using user ratings, demographics, and movie metadata to enhance user engagement and predict viewing preferences accurately.

🧾 Dataset Description

The project used three key datasets:

Ratings Data: User-movie interactions with ratings and timestamps (1M+ ratings from 6K+ users).

User Data: Demographics including gender, age, occupation, and zip code.

Movie Metadata: Movie titles with genres and release year.

🧪 Exploratory Data Analysis (EDA)

Most rated genre: Drama, followed by Comedy and Action.

Peak movie release period: 1990s, especially 1996.

Highest rating frequency: 4-star, majority of users: Male, age group: 25–34.

Popular professions: College students, Executives, and Academics.

Clear age-group preferences for genres were observed (e.g., 56+ prefer War/Documentary, Under 18 prefer Action/Adventure).

⚙️ Preprocessing & Feature Engineering

Parsed timestamps and extracted date features like year, month, day, and isWeekend.

Cleaned and formatted movie titles and genres; performed one-hot encoding for categorical features.

Addressed 0% missing data and eliminated duplicate entries.

🧠 Modeling Approaches

Memory-Based Collaborative Filtering

Pearson Correlation for item-item similarity.

Cosine Similarity for both item-item and user-user recommendations using Nearest Neighbors.

Generated top-N similar movie recommendations.

Model-Based Collaborative Filtering

Matrix Factorization using CMFRec:

Trained embedding models with d=4, evaluated on unseen data.

Achieved: RMSE = 0.86, MAPE = 26.2%

Extracted user-item latent factors for clustering and similarity analysis.

SVD using Surprise Library:

RMSE = 0.88, MAPE = 26.9%

Enabled scalable predictions and visualizations with PCA.

📈 Results & Visualizations

Generated 2D PCA plots for item and user embeddings to interpret clusters.

Created visual dashboards: Genre vs Age heatmaps, rating distributions, and occupational insights.

📊 Key Learnings

Matrix Factorization outperformed memory-based approaches in accuracy and scalability.

Incorporating demographics and genre metadata improved model interpretability.

Visualization of embeddings provided actionable user and content segmentation.

