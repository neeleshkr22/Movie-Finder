# Movie Finder 🎬

Movie Finder is a web application that allows users to search for movies, view trending films, and get details about their favorite films seamlessly. The app integrates with The Movie Database (TMDb) API for fetching movie data and uses Appwrite as a backend service for tracking search counts and trending movies.

## Features 🚀

- 🔍 **Movie Search**: Find movies using the TMDb API by searching with keywords.
- 📈 **Trending Movies**: Displays the most popular movies based on search activity.
- 🛠 **Debounced Search**: Optimized search performance using `react-use` debounce.
- 📡 **Real-time Updates**: Trending movies update dynamically based on user searches.
- 🌐 **Backend Integration**: Uses Appwrite for managing search counts and trending movie data.

## Tech Stack 🛠

### Frontend
- React.js
- Tailwind CSS
- React Hooks (`useState`, `useEffect`, `useDebounce`)

### Backend
- Appwrite (for database and API interactions)
- The Movie Database (TMDb) API

## Installation & Setup 🏗

### Prerequisites
- Node.js & npm/yarn installed
- TMDb API key (stored in `.env` as `VITE_TMDB_API_KEY`)
- Appwrite project setup

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/neeleshkr22/Movie-Finder.git
   cd movie-finder
   ```
2. Install dependencies:
   ```sh
   yarn install
   ```
3. Create a `.env` file and add your TMDb API key:
   ```sh
   VITE_TMDB_API_KEY=your_tmdb_api_key_here
   ```
4. Start the development server:
   ```sh
   yarn dev
   ```

## Usage 📖
1. Search for movies using the search bar.
2. View trending movies dynamically based on user search patterns.
3. Click on a movie to view details (extendable for more details in future versions).
4. Help in finding best movies based on IMDB rating

## API Integration 🔗

### TMDb API
- Used for fetching movie data (`discover/movie` and `search/movie` endpoints).
- API requests authenticated using Bearer Token stored in environment variables.

### Appwrite Backend
- `updateSearchCount(query, movie)`: Stores search counts and trending movie data.
- `getTrendingMovies()`: Retrieves top searched movies from Appwrite.


## Future Enhancements ✨
- 🎭 Movie details page with more metadata.
- 🎬 User authentication for personalized watchlists.
- ⭐ Ratings & Reviews feature using Appwrite backend.

## Contributing 🤝
Feel free to fork, create issues, and submit pull requests to improve this project!


---
Made with ❤️ by Neelesh
