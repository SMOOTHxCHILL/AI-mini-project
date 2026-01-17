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
```

## How to Run

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/content-based-news-recommendation.git
```

2. **Navigate to the project directory:**
```bash
cd content-based-news-recommendation
```

3. **Update the dataset path if required.**

4. **Run the script:**
```bash
python Content-Based\ News\ Recommendation\ Using\ TF-IDF\ and\ Cosine\ Similarity.py
```

5. **Enter an article index when prompted.**

## Sample Output
```bash
Because you liked:
[POLITICS] Senate passes major reform bill

You might also like:
- [POLITICS] Lawmakers debate new policy changes
- [POLITICS] Election reform gains momentum
- [POLITICS] Government announces legislative update
```
## License

This project is intended for educational and academic use.
