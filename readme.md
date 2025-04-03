# Movies Recommender System

## Overview
This project is a **Movie Recommendation System** built to suggest movies to users based on their preferences. It leverages the **TMDB Movie Dataset** to provide recommendations using various machine learning techniques. The system is designed to help users discover movies they might enjoy by analyzing movie metadata and user preferences.

## Features
- Content-based filtering to recommend movies similar to a selected movie.
- Use of cosine similarity to measure the closeness between movies.
- Interactive and user-friendly interface for selecting and recommending movies.

## Concepts and Technologies
### Concepts
1. **Content-Based Filtering**: Recommends movies based on their similarity to a selected movie using metadata like genres, keywords, and cast.
2. **Cosine Similarity**: Measures the similarity between two vectors (movies) in a multi-dimensional space.
3. **Natural Language Processing (NLP)**: Used for processing textual data like movie descriptions and keywords.

### Technologies
- **Python**: Core programming language for the project.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical computations.
- **Scikit-learn**: For implementing cosine similarity.
- **Streamlit**: For building the interactive web application.

## Dataset
The project uses the **TMDB Movie Dataset**, which contains metadata about movies such as titles, genres, cast, crew, and keywords.

- **Dataset Link**: [TMDB Movie Dataset](https://www.kaggle.com/tmdb/tmdb-movie-metadata)

## Project Structure
```
Movies-recommender-system/
│
├── data/                   # Contains the TMDB dataset
├── app.py                  # Main application file
├── recommender.py          # Logic for movie recommendations
├── requirements.txt        # Python dependencies
├── readme.md               # Project documentation
└── utils/                  # Helper functions and utilities
```

## How to Run the Project
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/Movies-recommender-system.git
    cd Movies-recommender-system
    ```

2. **Install Dependencies**:
    Ensure you have Python installed. Then, install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. **Download the Dataset**:
    - Download the TMDB Movie Dataset from the link above.
    - Place the dataset in the `data/` directory.

4. **Run the Application**:
    Start the Streamlit app:
    ```bash
    streamlit run app.py
    ```

5. **Interact with the Application**:
    Open the provided URL in your browser and start exploring movie recommendations.

## Logic Behind Recommendations
1. **Data Preprocessing**:
    - Extract relevant features like genres, keywords, and cast.
    - Combine these features into a single string for each movie.

2. **Vectorization**:
    - Convert the combined features into numerical vectors using TF-IDF or Count Vectorizer.

3. **Similarity Calculation**:
    - Compute cosine similarity between movie vectors to find similar movies.

4. **Recommendation**:
    - Sort movies based on similarity scores and return the top recommendations.

## Future Enhancements
- Add collaborative filtering for user-based recommendations.
- Integrate user ratings to improve recommendation accuracy.
- Deploy the application on a cloud platform for wider accessibility.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments
- [TMDB](https://www.themoviedb.org/) for providing the dataset.
- Open-source libraries and tools used in this project.

Feel free to contribute to this project by submitting issues or pull requests!