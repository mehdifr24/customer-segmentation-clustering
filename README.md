
# 🛍️ Customer Segmentation Using Machine Learning

## 📖 About

This project demonstrates an end-to-end unsupervised machine learning workflow for segmenting customers based on their purchasing behavior and demographic data. 
The project includes data exploration, preprocessing, feature scaling, determining the optimal number of clusters, and training multiple clustering algorithms to identify distinct customer profiles. This segmentation helps businesses tailor their marketing strategies and optimize campaigns.

## 🚀 Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* SciPy

## 📂 Dataset

The dataset contains information about mall customers, including their Age, Gender, Annual Income, and a calculated Spending Score (1-100). Since there are no pre-defined target labels, this is structured as an Unsupervised Learning problem.

## 📊 Project Workflow

* Data Understanding & Cleaning
* Exploratory Data Analysis (EDA) & Data Visualization
* Data Preprocessing & Feature Scaling (StandardScaler, LabelEncoder)
* Finding Optimal Clusters:
  * The Elbow Method
  * Dendrogram (Hierarchical Structure)
* Model Training & Implementation:
  * K-Means Clustering
  * Agglomerative Hierarchical Clustering
  * DBSCAN (Density-Based Clustering)
* Business Insights & Customer Profiling
* Quantitative Model Evaluation

## 📈 Model Performance

To evaluate the clustering algorithms without ground truth labels, intrinsic metrics such as the Silhouette Score (higher is better) and the Davies-Bouldin Index (lower is better) were used.

| Model | Silhouette Score | Davies-Bouldin Index |
| :--- | :---: | :---: |
| **K-Means (K=5)** | 0.304 | 1.167 |
| **Hierarchical (K=5)** | 0.287 | 1.220 |
| **DBSCAN** | 0.012 | 1.389 |

## 📊 Results Visualization

**1. Finding the Optimal K (Elbow Method & Dendrogram)**

<img width="698" height="474" alt="image" src="https://github.com/user-attachments/assets/a024d6ba-d07c-4a05-9909-dc5f1f723d7b" />


<img width="1011" height="621" alt="image" src="https://github.com/user-attachments/assets/03ee3cf2-5b30-4ef4-b70e-49a57a9e15e5" />

**2. Customer Segments (K-Means Output)**

<img width="984" height="584" alt="image" src="https://github.com/user-attachments/assets/1066bf27-36a1-41f0-b701-ecb832a40ea9" />


**3. Noise Detection (DBSCAN Output)**

<img width="988" height="590" alt="image" src="https://github.com/user-attachments/assets/7b1e401d-2c6b-4e7f-ba50-107052bbc712" />


## 🏆 Final Model Selection & Business Strategy

**K-Means (K=5)** was selected as the final model because it achieved the highest Silhouette Score and the lowest Davies-Bouldin Index, successfully dividing the customer base into 5 highly actionable segments:

1. **The Stars (High Income, High Spending):** Primary target for premium and personalized marketing.
2. **The Careful Savers (High Income, Low Spending):** Require value-driven promotions to be convinced to spend.
3. **The Standard Audience (Average Income & Spending):** Respond well to baseline loyalty programs.
4. **The Young Trendsetters (Low Income, High Spending):** Great targets for youth-oriented and social media marketing.
5. **The Conservative Seniors (Low Income, Low Spending):** Respond best to discounts and essential goods promotions.



## 👨‍💻 Author

Mehdi Ferdosi

Computer Science Student | Machine Learning Enthusiast

GitHub: https://github.com/mehdifr24
