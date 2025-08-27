# Customer Segmentation Analysis

## 📊 Project Overview

This project performs comprehensive customer segmentation analysis using machine learning clustering techniques on marketing campaign data. The goal is to identify distinct customer segments to enable targeted marketing strategies and improved customer relationship management.

## 🎯 Objective

**Main Goal:** Perform clustering analysis to summarize customer segments and identify patterns in customer behavior for strategic marketing decisions.

The analysis helps businesses:
- Understand their customer base better
- Tailor products according to specific customer needs and behaviors  
- Target marketing efforts more effectively
- Focus resources on customer segments most likely to purchase products

## 📈 Dataset Description

The dataset contains **2,240 customer records** with **29 features** covering customer demographics, purchase behavior, and marketing campaign responses.

### 🔍 Key Features

#### **Customer Demographics:**
- **ID:** Customer's unique identifier
- **Year_Birth:** Customer's birth year (converted to Age)
- **Education:** Customer's education level
- **Marital_Status:** Customer's marital status
- **Income:** Customer's yearly household income
- **Kidhome:** Number of children in household
- **Teenhome:** Number of teenagers in household
- **Dt_Customer:** Date of customer enrollment
- **Recency:** Days since last purchase

#### **Product Spending (Last 2 Years):**
- **MntWines:** Amount spent on wine
- **MntFruits:** Amount spent on fruits  
- **MntMeatProducts:** Amount spent on meat
- **MntFishProducts:** Amount spent on fish
- **MntSweetProducts:** Amount spent on sweets
- **MntGoldProds:** Amount spent on gold products

#### **Marketing Campaign Responses:**
- **AcceptedCmp1-5:** Binary indicators for campaign acceptance
- **Response:** Response to latest campaign
- **Complain:** Customer complaint in last 2 years

#### **Purchase Channels:**
- **NumWebPurchases:** Website purchases
- **NumCatalogPurchases:** Catalog purchases  
- **NumStorePurchases:** In-store purchases
- **NumDealsPurchases:** Discount purchases
- **NumWebVisitsMonth:** Monthly website visits

## 🛠️ Technical Implementation

### **Libraries & Tools:**
```python
- pandas, numpy          # Data manipulation
- matplotlib, seaborn    # Data visualization
- plotly                 # Interactive plotting
- scikit-learn          # Machine learning algorithms
- yellowbrick           # ML visualization
- kneed                 # Optimal cluster detection
```

### **Analysis Pipeline:**

#### 1. **Exploratory Data Analysis (EDA)**
- Dataset overview and structure analysis
- Missing value detection and handling
- Statistical summary and distribution analysis
- Correlation analysis between features
- Data type verification and cleaning

#### 2. **Data Preprocessing**
- Missing value imputation (Income column)
- Feature engineering:
  - Convert Year_Birth to Age
  - Create total spending feature (Spent)
  - Remove irrelevant columns (Z_CostContact, Z_Revenue)
- Data normalization and scaling
- Categorical variable encoding

#### 3. **Data Visualization**
- Correlation heatmaps
- Distribution plots
- Pair plots for key variables
- Feature relationship analysis

#### 4. **Dimensionality Reduction**
- **Principal Component Analysis (PCA)**
- Feature scaling using StandardScaler
- Variance explained analysis
- 3D visualization of principal components

#### 5. **Clustering Analysis**

##### **K-Means Clustering:**
- Elbow method for optimal cluster determination
- Silhouette score evaluation
- Cluster visualization and interpretation

##### **Hierarchical Clustering:**
- Dendrogram analysis
- Ward linkage method
- Optimal cluster detection using KneeLocator
- 3D cluster visualization

##### **DBSCAN Clustering:**
- Density-based clustering
- Noise point identification
- Parameter tuning (eps, min_samples)
- Silhouette score evaluation

## 📊 Key Results & Insights

### **Clustering Performance:**
- Multiple clustering algorithms implemented and compared
- Silhouette scores calculated for model evaluation
- 3D visualizations for cluster interpretation
- Optimal number of clusters determined through multiple methods

### **Customer Segments Identified:**
The analysis reveals distinct customer segments based on:
- **Spending Patterns:** High/Medium/Low spenders across product categories
- **Demographics:** Age, education, family composition
- **Channel Preferences:** Online vs. catalog vs. in-store shopping
- **Campaign Responsiveness:** Marketing engagement levels

### **Business Applications:**
- **Targeted Marketing:** Customize campaigns for each segment
- **Product Strategy:** Tailor product offerings to segment preferences  
- **Channel Optimization:** Focus resources on preferred customer channels
- **Customer Retention:** Identify high-value customer segments

## 📁 Project Structure

```
Customer_segmentation/
├── Market_Campaign.ipynb          # Main analysis notebook
├── marketing_campaign.csv         # Raw dataset
├── README.md                     # Project documentation
└── visualizations/               # Generated plots and charts
```

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd Customer_segmentation
   ```

2. **Install required packages:**
   ```bash
   pip install pandas numpy matplotlib seaborn plotly scikit-learn yellowbrick kneed
   ```

3. **Run the analysis:**
   ```bash
   jupyter notebook Market_Campaign.ipynb
   ```

## 💡 Key Findings

- **Multi-dimensional Analysis:** Successfully applied PCA to reduce dimensionality while preserving variance
- **Algorithm Comparison:** Evaluated multiple clustering approaches for robust segment identification
- **Actionable Insights:** Generated clear customer segments for strategic business decisions
- **Scalable Framework:** Created reusable methodology for ongoing customer analysis

## 🔧 Future Enhancements

- **Advanced Segmentation:** Implement ensemble clustering methods
- **Predictive Modeling:** Add customer lifetime value prediction
- **Real-time Analysis:** Develop automated segmentation pipeline
- **Interactive Dashboard:** Create business-friendly visualization interface
- **A/B Testing Framework:** Validate segment-based marketing strategies

## 📋 Requirements

```
Python 3.7+
pandas >= 1.0.0
numpy >= 1.18.0
matplotlib >= 3.0.0
seaborn >= 0.10.0
scikit-learn >= 0.22.0
plotly >= 4.0.0
yellowbrick >= 1.0.0
kneed >= 0.7.0
jupyter notebook
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request for:
- Code improvements
- Additional clustering algorithms
- Enhanced visualizations
- Documentation updates

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 📧 Contact

For questions, suggestions, or collaboration opportunities, please reach out through GitHub issues or pull requests.

---

**⭐ If you find this project helpful, please consider giving it a star!**
