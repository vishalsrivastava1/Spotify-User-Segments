# From Free to Premium: Understanding Spotify User Segments

## Project Overview
This project analyzes **Spotify user behavior data** to identify distinct user segments and understand **churn risk and premium conversion potential**. Using clustering techniques, the project profiles Free and Premium users based on listening behavior, engagement patterns, and contextual preferences to support **retention and conversion strategies**.

---

## Business Problem
Spotify faces two key challenges:
- **Reducing churn among Premium users**
- **Converting high-potential Free users to Premium**

The objective of this project is to:
- Identify meaningful user segments
- Understand behavioral differences between Free and Premium users
- Generate actionable insights to guide marketing and product strategies

---

## Data Source
- **Spotify User Behavior Dataset** (Kaggle)
- 520 survey-based observations
- Includes demographics, listening habits, mood influences, usage context, and subscription status

---

## Methodology

### 1. Data Cleaning & Transformation
- Corrected formatting issues caused by Excel auto-conversions
- Standardized missing and inconsistent values
- Encoded categorical variables for modeling compatibility

### 2. Feature Engineering
- Applied **split-and-explode transformations** to handle multi-value fields
  - Exploded rows with multiple entries in:
    - Music mood influences
    - Music listening context
- Preserved behavioral granularity by converting single-row multi-context users into multiple observations

### 3. User Segmentation
- Separated the dataset into **Free users** and **Premium users** to analyze revenue streams independently
- Applied **K-Means clustering** to both groups
- Used **Silhouette Score** to determine optimal number of clusters (K = 3)

### 4. Visualization & Interpretation
- Visualized cluster profiles using:
  - Heatmaps
  - Scatter plots
  - PCA-based projections
- Interpreted clusters to define actionable user personas

---

## Key Insights
- Free users show clear segmentation in premium willingness and engagement
- Certain Free user clusters demonstrate high conversion potential
- Premium users vary significantly in engagement and churn risk
- Context-driven and habit-based listening patterns strongly influence retention

---

## Business Recommendations
- Target high-potential Free user clusters with personalized Premium trials
- Improve early-stage Premium onboarding to reduce churn
- Align marketing campaigns with user listening contexts and engagement levels

---

## Tools & Technologies
- Python
- pandas, NumPy
- scikit-learn
- Matplotlib / Seaborn
- Excel

---

## My Contributions
- Transformed the dataset by **splitting and exploding rows with multiple entries** across two behavioral columns
- Structured the data to retain full behavioral context for clustering
- **Separated the dataset into Free and Premium users** for independent analysis
- Supported clustering analysis through data preparation
- Created visualizations and **derived insights to answer key business questions**
- Contributed to actionable recommendations for churn reduction and conversion

---

## Team Members
- Christie Shin
- Shivani Vallamdas
- Gema Zhu
- Vishal Srivastava
- Shuai Zhao

---

## Future Work
- Incorporate time-based behavioral data
- Apply predictive churn models
- Integrate streaming history for deeper personalization insights

