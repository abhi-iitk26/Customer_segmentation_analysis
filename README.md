# 📊 Customer Segmentation Analysis

## 🎯 Project Overview
This project performs customer segmentation analysis using machine learning clustering techniques on marketing campaign data to identify distinct customer segments for targeted marketing strategies.

## 📁 Dataset
- **Records:** 2,240 customers
- **Features:** 29 attributes including demographics, purchase behavior, and campaign responses

### Key Features:
- **Demographics:** Age, Education, Income, Marital Status, Family Size
- **Product Spending:** Wines, Fruits, Meat, Fish, Sweets, Gold Products
- **Purchase Channels:** Web, Catalog, Store, Deals
- **Campaign Response:** Acceptance rates for 5 campaigns
- **Behavior:** Recency, Website visits, Complaints

## 🛠️ Technologies Used
- **Python Libraries:** pandas, numpy, matplotlib, seaborn, plotly
- **Machine Learning:** scikit-learn, yellowbrick, kneed
- **Techniques:** PCA, K-Means, Hierarchical Clustering, DBSCAN

## 📈 Analysis Pipeline

1. **Exploratory Data Analysis (EDA)**
   - Data cleaning and preprocessing
   - Statistical analysis and visualization
   - Correlation analysis

2. **Feature Engineering**
   - Age calculation from birth year
   - Total spending aggregation
   - Missing value imputation

3. **Dimensionality Reduction**
   - Principal Component Analysis (PCA)
   - Feature scaling and normalization

4. **Clustering Models**
   - K-Means Clustering (Elbow method)
   - Hierarchical Clustering (Dendrogram)
   - DBSCAN (Density-based)
   - Silhouette score evaluation

## 🔍 Key Insights
- Identified distinct customer segments based on spending patterns and demographics
- Analyzed customer preferences across purchase channels
- Evaluated campaign responsiveness by segment
- Provided actionable insights for targeted marketing

## 🚀 How to Run
```bash
# Clone repository
git clone <repository-url>

# Install dependencies
pip install pandas numpy matplotlib seaborn plotly scikit-learn yellowbrick kneed

# Run notebook
jupyter notebook Market_Campaign.ipynb
```

## 📊 Results
- Multiple clustering algorithms compared for optimal segmentation
- 3D visualizations of customer clusters
- Clear identification of high-value customer segments
- Data-driven recommendations for marketing strategy

## 💡 Business Applications
- Personalized marketing campaigns
- Product recommendation optimization
- Channel strategy improvement
- Customer retention focus

## 📋 Project Structure
```
Customer_segmentation/
├── Market_Campaign.ipynb
├── marketing_campaign.csv
└── README.md
```

---

⭐ **Star this repository if you found it useful!**
