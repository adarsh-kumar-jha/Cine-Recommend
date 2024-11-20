# 🎥 Movies/Cinema Recommendation System  

Welcome to the **Cine-Recommend**! This project is a content-based recommendation engine that suggests movies based on user preferences. The system utilizes advanced natural language processing techniques to analyze movie metadata and provide accurate and personalized recommendations.

---

## 🛠 Features  

- **Content-Based Filtering**: Recommends movies similar to the one you like by analyzing metadata such as genres, cast, crew, and keywords.  
- **Efficient Data Processing**: Handles missing data, duplicate entries, and textual data cleaning for optimal performance.  
- **Similarity Calculation**: Uses **Cosine Similarity** and vectorized movie tags for precise movie comparisons.  
- **Interactive Recommendations**: Simple Python-based interface for users to input their favorite movie and receive tailored suggestions.  

---

## 📂 Dataset  

The project uses the **TMDB 5000 Movies Dataset**, consisting of two primary files:  
1. **tmdb_5000_movies.csv**: Contains movie details such as title, genres, keywords, and overview.  
2. **tmdb_5000_credits.csv**: Includes cast and crew information.  

---

## 🚀 How It Works  

### 1. **Data Preprocessing**  
- Extracted essential columns such as `genres`, `keywords`, `cast`, `crew`, and `overview`.  
- Cleaned the data by removing null values and duplicates.  
- Processed JSON-like data into structured Python lists for easy manipulation.  

### 2. **Feature Engineering**  
- Created a unified `tags` column by combining cleaned metadata for each movie.  
- Applied **stemming** and removed stop words to normalize text data.  

### 3. **Similarity Computation**  
- Transformed movie tags into feature vectors using **CountVectorizer**.  
- Calculated similarity scores using **Cosine Similarity** to compare movies.  

### 4. **Recommendation Engine**  
- Built a function to find and display the top 5-10 most similar movies for a given input movie title.  

---

## 📊 Technology Stack  

- **Programming Language**: Python  
- **Libraries Used**:  
  - `pandas` and `numpy` for data manipulation  
  - `nltk` for natural language processing  
  - `scikit-learn` for vectorization and similarity computation  

---

## 🔧 Installation and Usage  

1. **Clone the Repository**  
   ```bash  
   git clone https://github.com/your-username/movie-recommendation-system.git  
   cd movie-recommendation-system  
   ```  

2. **Install Dependencies**  
   Ensure you have Python installed, then install the required libraries:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. **Run the Project**  
   Execute the Python script to test the recommendation system:  
   ```bash  
   python main.py  
   ```  

4. **Input a Movie**  
   Type a movie title to get recommendations. Example:  
   ```bash  
   Enter movie name: Batman  
   Recommended movies:  
   - Batman Begins  
   - The Dark Knight  
   - Justice League  
   - Batman v Superman: Dawn of Justice  
   - The Dark Knight Rises  
   ```  

---

## 📈 Future Enhancements  

- **Graphical User Interface (GUI)** for improved user experience.  
- Integrate collaborative filtering for user-based recommendations.  
- Expand the dataset to include more movies and metadata.  

---

## 🤝 Contributing  

Contributions are welcome! Feel free to:  
- Open issues for bugs or feature requests.  
- Fork the repository and submit a pull request.  

---
  

- [The Movie Database (TMDB)](https://www.themoviedb.org/) for providing the dataset.  
- Open-source contributors for the libraries used in this project.  

---

Let me know if you'd like further customization or additions!
