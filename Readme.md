🛒 Smart Cart – E-commerce Customer Segmentation

📌 Project Overview

Smart Cart is an Unsupervised Machine Learning project focused on segmenting e-commerce customers based on their characteristics and purchasing behavior.

The project uses customer data to identify meaningful groups through clustering algorithms. These segments can help businesses understand their customers, develop targeted marketing strategies, improve customer retention, and personalize shopping experiences.

The complete workflow includes data preprocessing, feature engineering, correlation analysis, PCA-based visualization, cluster evaluation, model comparison, and customer segment profiling.

🎯 Objectives

- Identify meaningful customer segments using clustering algorithms.
- Handle missing values and encode categorical features.
- Perform feature engineering to improve the dataset.
- Analyze feature relationships using a correlation heatmap.
- Apply PCA and 3D visualization to explore customer patterns.
- Determine the optimal number of clusters using the Elbow Method and Silhouette Score.
- Compare K-Means and Agglomerative Clustering.
- Select the most suitable clustering algorithm.
- Summarize and interpret customer segments using Pandas "groupby()" and "mean()".

🛠️ Technologies Used

- Python
- Pandas – Data manipulation and analysis
- NumPy – Numerical computations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization and correlation heatmaps
- Scikit-learn – PCA and clustering algorithms
- Jupyter Notebook – Development and experimentation

📂 Project Structure

Smart-Cart-Customer-Segmentation/
│
├── smartcart_customers.csv
├── smartcart.ipynb
├── README.md
└── requirements.txt

🔄 Project Workflow

1. Data Loading and Exploration

- Loaded the dataset "smartcart_customers.csv".
- Explored the dataset structure, columns, data types, and statistical properties.
- Identified missing values and examined the available customer features.

2. Data Preprocessing

- Handled missing values.
- Encoded categorical variables into numerical representations.
- Prepared the dataset for machine learning algorithms.

3. Feature Engineering

- Created or transformed relevant features for customer analysis.
- Prepared the feature set for dimensionality reduction and clustering.

4. Correlation Analysis

- Generated a correlation matrix to examine relationships between numerical features.
- Visualized the correlations using a heatmap.
- Used the heatmap to understand feature relationships and potential redundancy.

5. Dimensionality Reduction and Visualization

- Applied Principal Component Analysis (PCA) to reduce dimensionality.
- Created 3D visualizations to explore customer distribution and potential cluster patterns.

6. Finding the Optimal Number of Clusters

Used two evaluation techniques to identify a suitable number of clusters.

Elbow Method

- Calculated Within-Cluster Sum of Squares (WCSS) for different values of K.
- Plotted WCSS against the number of clusters.
- Examined the elbow point to identify a suitable cluster count.

Silhouette Score

- Calculated silhouette scores for different clustering configurations.
- Evaluated cluster cohesion and separation.
- Used the scores alongside the Elbow Method to select the final number of clusters.

Optimal number of clusters: K = 4

7. Clustering Model Comparison

K-Means Clustering

- Applied K-Means to group customers into four clusters.
- Analyzed the resulting clusters using evaluation metrics and visualizations.

Agglomerative Clustering

- Applied hierarchical clustering to identify groups of similar customers.
- Analyzed the resulting customer segments and compared them with K-Means.

Final Model Selected: Agglomerative Clustering

Agglomerative Clustering was selected as the preferred approach based on the comparative analysis performed in the project.

8. Customer Segment Analysis

After performing clustering:

- Assigned cluster labels to customers.
- Grouped customer records by cluster using Pandas "groupby()".
- Calculated the mean of relevant features for each cluster.
- Compared the resulting summaries to understand differences between customer segments.

This step makes the clustering results easier to interpret and helps translate them into potential business insights.

📊 Key Analysis and Visualizations

- Correlation heatmap
- PCA-based dimensionality reduction
- 3D customer visualization
- Elbow Method plot using WCSS
- Silhouette Score analysis
- K-Means clustering results
- Agglomerative Clustering results
- Customer segment summary using grouped mean statistics

💡 Business Applications

The resulting customer segments can support:

- Targeted Marketing: Create campaigns for different customer groups.
- Personalization: Tailor product recommendations to customer characteristics.
- Customer Retention: Design engagement strategies for different segments.
- Customer Insights: Understand differences in customer behavior.
- Marketing Optimization: Allocate marketing resources based on segment characteristics.

These are potential applications of the analysis; their effectiveness should be validated against actual business outcomes.

🚀 How to Run the Project

Prerequisites

Install Python and the required libraries:

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

Execution Steps

1. Clone or download this repository.

2. Ensure "smartcart_customers.csv" and "smartcart.ipynb" are in the expected locations.

3. Launch Jupyter Notebook:
   
   jupyter notebook

4. Open "smartcart.ipynb".

5. Run the notebook cells sequentially to reproduce the preprocessing, visualization, clustering, and customer segment analysis.

🔮 Future Improvements

- Create detailed customer personas for each cluster.
- Explore DBSCAN and other clustering algorithms.
- Experiment with different linkage methods and distance metrics.
- Evaluate cluster stability and robustness.
- Develop an interactive dashboard using Streamlit.
- Build segment-specific marketing and recommendation strategies.

🏁 Conclusion

The Smart Cart project demonstrates the application of unsupervised machine learning to e-commerce customer segmentation. It combines data preprocessing, feature engineering, correlation analysis, PCA visualization, and clustering evaluation to discover meaningful customer groups.

Using the Elbow Method and Silhouette Score, four clusters (K = 4) were selected for the analysis. After comparing K-Means and Agglomerative Clustering, Agglomerative Clustering was chosen as the preferred model. Finally, cluster-wise summaries using Pandas "groupby()" and "mean()" helped interpret the characteristics of the identified customer segments.

---

Project Name: Smart Cart – E-commerce Customer Segmentation
Domain: Data Science | Machine Learning | E-commerce Analytics
Learning Approach: Unsupervised Learning
Optimal Cluster Count: K = 4
Selected Algorithm: Agglomerative Clustering