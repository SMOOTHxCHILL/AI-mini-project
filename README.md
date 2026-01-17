# AI mini-project: Content-Based News Recommendation System  
### Using TF-IDF and Cosine Similarity

This project implements a **content-based news recommendation system** using **Natural Language Processing (NLP)** techniques. It recommends news articles based on textual similarity between headlines and short descriptions.

The system leverages **TF-IDF vectorization** and **cosine similarity** to find articles that are semantically similar to a user-selected article, constrained within the same news category.

---

## Features

- TF-IDF (Term Frequency–Inverse Document Frequency) for text representation  
- Cosine similarity to measure article similarity  
- Category-aware recommendations  
- Simple command-line interface (CLI)  
- Scalable to large datasets

---

## Approach

1. **Data Loading**
   - Loads the HuffPost News dataset from a JSON file
   - Combines `headline` and `short_description` into a single text field

2. **Text Vectorization**
   - Converts article text into numerical vectors using TF-IDF
   - Removes stop words and limits vocabulary size

3. **User Interaction**
   - Displays a random sample of articles
   - User selects an article they like

4. **Similarity Computation**
   - Computes cosine similarity within the same category
   - Returns the top most similar articles

---

## Dataset

- **Name:** HuffPost News Category Dataset (v3)
- **Format:** JSON (line-delimited)
- **Fields Used:**
  - `headline`
  - `short_description`
  - `category`

Ensure the dataset path in the script matches your local file system.

---

## Requirements

Install the required dependencies:

```bash
pip install pandas scikit-learn numpy
