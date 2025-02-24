# Movie Recommendation System

## Description
A content-based movie recommendation system that suggests movies based on user text descriptions using TF-IDF vectorization and cosine similarity.

## Demo
<video src="https://github.com/Hotragn/lumaa-spring-2025-ai-ml/blob/main/Demo.mp4" controls="controls" style="max-width: 730px;">
</video>


## Salary Expectation
$3000 per month

## Dataset
- **Source**: [https://www.kaggle.com/datasets/moazeldsokyx/the-500-best-movies-imdb]
- **Size**: [503] movies
- **Features**: Movie Name |	Rating |	Runtime |	Genre	Metascore |	Plot |	Directors |	Stars |	Votes |	Gross |	Link
- **Format**: CSV file

## Setup Instructions

### Prerequisites
- Python 
- VScode/Jupyter Notebook/Colab

### Installation
1. Clone the repository
   ```sh
   git clone [your-repository-url]
   cd [repository-name]
   ```

2. Create virtual environment
   ```sh
   python -m venv venv
   ```

3. Activate virtual environment
   - **Windows**
     ```sh
     venv\Scripts\activate
     ```
   - **Linux/Mac**
     ```sh
     source venv/bin/activate
     ```

4. Install dependencies
   ```sh
   pip install -r requirements.txt
   ```

## Required Libraries
```txt
numpy==1.21.0
pandas==1.3.0
scikit-learn==0.24.2
```

## Usage

### Command Line
```sh
python recommend.py "I love thrilling action movies set in space"
```

### Python Interface
```python
After running all the cells we can test it:

user_query = "I love animation and action movies"
recommendations = get_recommendations(user_query, df)
```

## Example Output
**Input:**
```txt
"I love animation and action movies"
"
```

**Recommendations:**
```txt
User Query: I love animation and action movies

Recommended Movies:

1. The Incredibles
Genre: Animation, Action, Adventure
Similarity Score: 0.30

2. Mononoke-hime
Genre: Animation, Action, Adventure
Similarity Score: 0.30

3. Beauty and the Beast
Genre: Animation, Family, Fantasy
Similarity Score: 0.21

4. The Little Mermaid
Genre: Animation, Adventure, Family
Similarity Score: 0.21

5. Being John Malkovich
Genre: Comedy, Drama, Fantasy
Similarity Score: 0.11
```

## Implementation Details

### Key Features
- TF-IDF vectorization for text processing
- Lemmatization to improve matching similarity
- Cosine similarity for recommendation matching
- Genre-based filtering
- Basic Preprocessed text analysis

### Functions
- `preprocess_text()`: Cleans and normalizes text data
- `create_tfidf_matrix()`:Creates a tfidf valued matrix for each sentence/word passed
- `compute_similarity()`:Finalizes the similariy matrix using cosine similarity calculation
- `get_recommendations()`: Generates movie recommendations
- `extract_genre()`: Extracts genre preferences from query

## Project Structure
```
movie-recommender/
└── Demo.mp4
└── Top_Movies.csv
├── Simple Content-Based Recommendation.ipynb
│  
├── requirements.txt
└── README.md
```

## Performance
- **Response Time**: < 2 seconds
- **Memory Usage**: In Kbs
- **Dataset Size**: [503] movies

## Author
[Hotragn Pettugani]
- GitHub: [@hotragn]
- LinkedIn: [https://www.linkedin.com/in/hotragn-pettugani/]
