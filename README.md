# Cosmetics Ingredient-Based Recommendation System

## Overview
This project applies data science techniques to help users choose cosmetic products based on their ingredients. Many people struggle to understand complex ingredient lists and may experience skin reactions when trying new products. This project aims to solve this problem by building a **content-based recommendation system** that analyzes ingredient similarity among different cosmetic products.

## Key Features
- **Ingredient-Based Similarity:** Uses **word embeddings** and **t-SNE** to analyze ingredient compositions.
- **Visual Representation:** Applies **t-SNE for dimensionality reduction** and visualizes products with **Bokeh interactive plots**.
- **One-Hot Encoding for Ingredients:** Transforms ingredient lists into a binary document-term matrix (DTM).
- **Filtering by Skin Type & Product Category:** Users can filter recommendations based on their skin type and desired product category.
- **Hover Tool for Product Info:** Allows users to explore products interactively with additional details such as brand, price, and rating.

## Dataset
The dataset contains **1,472 cosmetic products** from Sephora, categorized into:
- **Moisturizers**
- **Cleansers**
- **Face Masks**
- **Eye Creams**
- **Sun Protection**

Each product includes details such as ingredients, price, brand, and user ratings.

## Methodology
1. **Data Preprocessing**
   - Load dataset and filter by product category and skin type.
   - Tokenize ingredient lists and convert them into a structured format.
   
2. **Feature Engineering**
   - Build a **document-term matrix (DTM)** using one-hot encoding.
   - Reduce dimensionality using **t-SNE** to visualize similarities.
   
3. **Visualization with Bokeh**
   - Create an **interactive scatter plot** to map cosmetic products.
   - Add a **hover tool** to display product information.

## Installation & Dependencies
To run this project, install the following Python libraries:
```bash
pip install pandas numpy scikit-learn bokeh
```

## Usage
1. Clone the repository:
```bash
git clone https://github.com/your-username/cosmetic-recommender.git
cd cosmetic-recommender
```
2. Run the Jupyter Notebook or Python script.
3. Explore the Bokeh visualization and find similar cosmetic products!

## Future Improvements
- Implement **TF-IDF or Word2Vec** instead of one-hot encoding for better ingredient representation.
- Enhance recommendation logic with **cosine similarity or clustering**.
- Incorporate **user preferences** to make personalized recommendations.


