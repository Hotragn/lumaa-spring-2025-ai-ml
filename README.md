# Movie Recommendation System

## Description
A content-based movie recommendation system that suggests movies based on user text descriptions using TF-IDF vectorization and cosine similarity.

## Demo
[Link to your video demo]

## Salary Expectation
[Your expected salary per month]

## Dataset
- **Source**: [Dataset source name/link]
- **Size**: [Number] movies
- **Features**: Movie titles, plots, genres
- **Format**: CSV file

## Setup Instructions

### Prerequisites
- Python 3.8+
- pip package manager

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
from recommender import get_recommendations

query = "I love thrilling action movies set in space"
recommendations = get_recommendations(query, n_recommendations=5)
```

## Example Output
**Input:**
```txt
"I love thrilling action movies set in space"
```

**Recommendations:**
```txt
Guardians of the Galaxy
Genre: Action, Sci-Fi, Comedy
Similarity Score: 0.856

Star Wars: A New Hope
Genre: Sci-Fi, Action, Adventure
Similarity Score: 0.789

Interstellar
Genre: Sci-Fi, Drama, Adventure
Similarity Score: 0.745
```

## Implementation Details

### Key Features
- TF-IDF vectorization for text processing
- Cosine similarity for recommendation matching
- Genre-based filtering
- Preprocessed text analysis

### Functions
- `preprocess_text()`: Cleans and normalizes text data
- `get_recommendations()`: Generates movie recommendations
- `extract_genre()`: Extracts genre preferences from query

## Project Structure
```
movie-recommender/
├── data/
│   └── movies.csv
├── src/
│   ├── recommender.py
│   └── utils.py
├── requirements.txt
└── README.md
```

## Performance
- **Response Time**: < 2 seconds
- **Memory Usage**: < 500MB
- **Dataset Size**: [Number] movies

## Author
[Your Name]
- GitHub: [@username]
- LinkedIn: [Your LinkedIn]

## License
MIT License

## Acknowledgments
- Dataset provided by [Source]
- Inspired by content-based recommendation systems
