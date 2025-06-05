# Movie Recommendation System

A content-based movie recommendation system built with Python and Streamlit that suggests similar movies based on your selection.

## 🎬 Features

- **Interactive Web Interface**: Clean and intuitive Streamlit-based UI
- **Content-Based Filtering**: Recommends movies based on similarity metrics
- **Real-time Recommendations**: Get 5 movie suggestions instantly
- **Search & Select**: Type or select movies from a comprehensive dropdown

## 🚀 How It Works

The system uses content-based collaborative filtering to analyze movie features and calculate similarity scores between different movies. When you select a movie, the algorithm finds the 5 most similar movies based on pre-computed similarity matrices.

## 📋 Prerequisites

- Python 3.7+
- Required Python packages (see Installation section)

## 🛠️ Installation

1. Clone this repository:
```bash
git clone <https://github.com/Vivek3500/Movie-Recommendation-System.git>
cd movie-recommendation-system
```

2. Install required packages:
```bash
pip install streamlit pandas pickle-mixin requests
```

3. Ensure you have the required data files in your project directory:
   - `movie_dict.pkl` - Preprocessed movie dataset
   - `similarity.pkl` - Pre-computed similarity matrix

## 📊 Dataset

This project uses the **TMDb Movie Metadata** dataset from Kaggle:
- **Source**: [TMDb Movie Metadata](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
- **Description**: Comprehensive movie database with metadata including genres, cast, crew, and more

## 🏃‍♂️ Usage

1. Run the Streamlit application:
```bash
streamlit run app.py
```

2. Open your web browser and navigate to the provided local URL (typically `http://localhost:8501`)

3. Select a movie from the dropdown menu or start typing to search

4. Click "Show Recommendation" to get 5 similar movie suggestions

## 📁 Project Structure

```
movie-recommendation-system/
│
├── app.py                 # Main Streamlit application
├── movie_dict.pkl         # Processed movie dataset
├── similarity.pkl         # Pre-computed similarity matrix
├── DatasetLink.txt        # Link to original dataset
└── README.md             # Project documentation
```

## 🔧 Code Overview

### Main Components:

- **`recommend(movie)`**: Core recommendation function that finds similar movies
- **Streamlit Interface**: User-friendly web interface for movie selection
- **Pickle Data Loading**: Efficient loading of preprocessed data

### Algorithm Flow:
1. User selects a movie from the dropdown
2. System finds the movie's index in the dataset
3. Retrieves similarity scores for that movie
4. Sorts and selects top 5 most similar movies
5. Returns movie titles as recommendations

## 🎯 Future Enhancements

- [ ] Add movie posters and descriptions
- [ ] Implement hybrid recommendation (collaborative + content-based)
- [ ] Include user ratings and reviews
- [ ] Add movie trailers and links
- [ ] Implement user preference learning
- [ ] Add genre-based filtering options

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [The Movie Database (TMDb)](https://www.themoviedb.org/) for providing the dataset
- [Streamlit](https://streamlit.io/) for the amazing web framework
- [Kaggle](https://www.kaggle.com/) for hosting the dataset

## 📞 Contact

For questions or suggestions, please feel free to reach out or create an issue in this repository.

---

*Happy movie watching! 🍿*
