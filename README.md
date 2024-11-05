# AIE425 Intelligent Recommender Systems - Assignment #1: Neighborhood Collaborative Filtering Models

### Student Information
- **Student ID**: A20001136
- **Full Name**: Abdelrahman El-Sayyad

---

## Table of Contents
1. [Introduction](#introduction)
2. [Core Idea of the Assignment](#core-idea-of-the-assignment)
3. [Dataset Description](#dataset-description)
4. [Data Collection and Preprocessing](#data-collection-and-preprocessing)
5. [Methodology and Implementation](#methodology-and-implementation)
6. [Assignment Results](#assignment-results)
7. [Conclusion and Opinion](#conclusion-and-opinion)
8. [References](#references)

---

### Introduction
This assignment explores the fundamental concepts of Intelligent Recommender Systems, focusing on user-based and item-based Neighborhood Collaborative Filtering (CF) models. Using data scraping techniques, this project involves building and analyzing a user-item matrix to generate recommendations.

### Core Idea of the Assignment
The objective is to develop collaborative filtering algorithms (both user-based and item-based) through data collection from a web source, transforming this data into a user-item matrix, and calculating recommendations based on similarity measures.

### Dataset Description
- **Source**: Data scraped from "quotes.toscrape.com".
- **Columns**:
  - `Quote`: Text of the quote.
  - `Author`: Name of the author.
  - `Tags`: Keywords or "genres" associated with each quote, representing themes.

- **Data Structure**: 
  - Each row represents a simulated user.
  - Each column represents a unique "tag" from the scraped quotes.
  - Each cell contains a rating from 1 to 5, representing hypothetical user preferences.

### Data Collection and Preprocessing
Data was collected using Python's BeautifulSoup library, scraping quotes, authors, and tags from multiple pages on the quotes website. The tags extracted from each quote serve as item features in the user-item matrix.

**User-Item Matrix**: Simulated with random ratings (1 to 5) to serve as the dataset for collaborative filtering.

### Methodology and Implementation
1. **Collaborative Filtering (CF) Models**:
   - **User-Based CF**: Finds similar users to make recommendations.
   - **Item-Based CF**: Finds similar items for recommendation.

2. **Similarity Measures**:
   - **Cosine Similarity** and **Pearson Correlation Coefficient** were used to calculate user-user and item-item similarities.

3. **Rating Prediction**:
   - Predictions were calculated using similarity matrices to suggest items with high relevance to each user.

### Assignment Results
1. **Average Ratings**:
   - Calculated for each tag across users to understand general preferences.

2. **Cosine Similarity vs. Pearson Correlation**:
   - **Cosine Similarity**: Focuses on angular similarity, useful for general pattern matching.
   - **Pearson Correlation**: Adjusts for rating biases, capturing more nuanced user/item relationships.

3. **Top-N Recommendations**:
   - Based on cosine similarity for user and item approaches, top-5 items were recommended to each user.

### Conclusion and Opinion
User-based CF is suitable for datasets with many users but fewer items, while item-based CF works well for static catalogs. Pearson correlation offers finer analysis, while cosine similarity is simpler for general recommendations.

### References
1. BeautifulSoup Documentation: [https://www.crummy.com/software/BeautifulSoup/bs4/doc/](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
2. Scikit-learn Cosine Similarity Documentation: [https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html)
3. Quotes to Scrape: [http://quotes.toscrape.com](http://quotes.toscrape.com)
4. OpenAI's ChatGPT: Assistance in generating, formatting, and structuring content.

---

Please refer to each section of the report for a detailed analysis and code implementation.
