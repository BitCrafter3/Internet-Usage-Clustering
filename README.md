Introduction
This project aims to group internet users based on their browsing habits. Clustering allows us to analyze users with similar usage patterns, which is helpful in behavior prediction, service customization, and anomaly detection. We use KMeans clustering for this unsupervised learning task, based on three key attributes: time spent online daily, variety of sites visited, and the number of sessions per day
Methodology
a. Dataset
The dataset used contains:
•	daily_usage_hours: Time (in hours) spent online per day.
•	site_categories_visited: Number of different categories of websites accessed.
•	sessions_per_day: Count of browsing sessions per day.
b. Data Preprocessing
All features were standardized using StandardScaler from scikit-learn to remove scale-related bias in clustering.
c. Clustering Algorithm
We used KMeans, a centroid-based unsupervised learning algorithm.
•	The Elbow Method helped determine the optimal number of clusters (k=3).
•	Model initialized with random_state=42 for reproducibility.
d. Evaluation
The Silhouette Score was used to measure how well samples were clustered with similar ones, with a value of 0.30 indicating reasonable separation.
e. Visualization
Clusters were plotted on a 2D scatter plot using matplotlib and seaborn. The plot visualized session frequency vs daily usage time for each user
