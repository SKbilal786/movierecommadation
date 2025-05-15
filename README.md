# Movie Recommender System

This is a web-based Movie Recommender System built using **Python**, **Streamlit**, and the **TMDb API**. It suggests movies similar to a selected title based on content similarity. The application leverages machine learning to provide movie recommendations and displays posters of the recommended movies.

## Features

* Select a movie from a dropdown list
* Get top 5 similar movie recommendations
* View movie posters alongside the recommendations
* Simple, interactive UI built with Streamlit

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/movie-recommender.git
   cd movie-recommender
   ```

2. Install required packages:

   ```bash
   pip install streamlit requests pandas pickle
   ```

3. Make sure you have the following files:

   * `movie_list.pkl`: A pickled DataFrame containing movie titles and IDs.
   * `similarity.pkl`: A pickled similarity matrix for movies.

4. Run the application:

   ```bash
   streamlit run app.py
   ```

## Usage

* Open the local Streamlit server in your browser (usually at `http://localhost:8501`).
* Select a movie from the dropdown menu.
* Click on 'Show Recommendation' to view similar movies and their posters.

## API Configuration

The app uses the TMDb API to fetch movie posters. Ensure that you have a valid API key and replace it in the `fetch_poster` function within `app.py`.

## Troubleshooting

* **Connection Errors:** Check your internet connection and ensure the TMDb API key is correct.
* **Poster Not Found:** The app will display a placeholder image if the poster is not available.
* **App Crashes:** Make sure you have the correct version of the `requests` library installed.

## License

This project is licensed under the MIT License.

## Acknowledgements

* [TMDb API](https://www.themoviedb.org/documentation/api) for providing movie data.
* [Streamlit](https://streamlit.io) for the web interface.
