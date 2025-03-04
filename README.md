<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FilmFlix - Movies and TV Shows</title>
    <style>
        /* Reset some basic styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body and general layout */
        body {
            font-family: Arial, sans-serif;
            background-image: url('');
            width: 100;
            color: #0e4b11;
        }

        /* Header */
        header {
            display: flex;
            justify-content: space-between;
            padding: 50px;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 10;
        }

        header .logo h1 {
            font-size: 50px;
            color: #e50914;
        }

        header .nav ul {
            display: flex;
            list-style-type: none;
        }

        header .nav ul li {
            margin: 0 15px;
        }

        header .nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 16px;
            padding: 10px 15px;
        }

        header .nav ul li a:hover {
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 5px;
        }

        /* Search Bar */
        .search-bar {
            display: flex;
            align-items: center;
        }

        .search-bar input {
            padding: 8px 15px;
            font-size: 16px;
            border-radius: 5px;
            border: 1px solid #333;
            background-color: hsl(0, 0%, 0%);
            color: white;
        }

        .search-bar button {
            padding: 8px 15px;
            margin-left: 10px;
            font-size: 20px;
            background-color: hwb(253 4% 37%);
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }

        .search-bar button:hover {
            background-color: #f40612;
        }

        /* Main Banner */
        .main-banner {
            background: url('https://via.placeholder.com/1500x600') no-repeat center center/cover;
            height: 600px;
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
            color: hsl(0, 83%, 40%);
        }

        .main-banner .banner-content {
            text-align: center;
        }

        .main-banner h2 {
            font-size: 100px;
            font-weight: bold;
            color: #c20817;
        }

        .main-banner p {
            font-size: 20px;
            margin-top: 10px;
        }

        .main-banner button {
            padding: 10px 20px;
            margin: 10px 15px;
            font-size: 16px;
            border: none;
            background-color: hsl(241, 75%, 55%);
            color: hsl(0, 33%, 1%);
            cursor: pointer;
            border-radius: 5px;
        }

        .main-banner {
            background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTJJck36TCecZ1Q4AfrK2usMxvf-OJNNVYHSiiHz6aapLA7mrLYkVqzCelj6KbyzjfBPh4&usqp=CAU');
            background-repeat: no-repeat;
            background-attachment: fixed; 
            background-size: 100% 100%;
        }

        /* Featured Movies Section */
        .featured-movies {
            margin-top: 150px;
            padding: 20px;
        }

        .featured-movies h2 {
            font-size: 32px;
            margin-bottom: 20px;
        }

        .movie-list {
            display: flex;
            gap: 15px;
            overflow-x: auto;
            padding-bottom: 20px;
        }

        .movie-item {
            flex: 0 0 300px;
            text-align: center;
            position: relative;
            transition: transform 0.3s;
        }

        .movie-item:hover {
            transform: scale(1.05);
        }

        .movie-item img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 4px 10px #db5f5fb3;
        }

        .movie-item .movie-info {
            position: absolute;
            bottom: 20px;
            left: 0;
            right: 0;
            background: hwb(0 0% 100% / 0.6);
            padding: 10px;
            border-radius: 5px;
            opacity: 0;
            transition: opacity 0.3s;
        }

        .movie-item:hover .movie-info {
            opacity: 1;
        }

        .movie-item h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .movie-item p {
            font-size: 14px;
        }

        /* Footer */
        footer {
            padding: 20px;
            text-align: center;
            background-color: #141414;
            margin-top: 50px;
        }
    </style>
</head>
<body>
    <!-- Header Section -->
    <header>
        <div class="logo">
            <h1>FilmFlix</h1>
        </div>
        
        <!-- Search Bar -->
        <div class="search-bar">
            <input type="text" placeholder="Search for movies or TV shows..." id="search">
            <button id="search-btn">Search</button>
        </div>
    </header>

    <!-- Main Banner -->
    <section class="main-banner">
        <div class="banner-content">
            <h1>ወደ አማርኛ የተተረጎሙ ፊልሞች</h1>
            <h3>FilmFlix</h3>
        </div>
    </section>
    <marquee>
      
   </marquee>

    <!-- Featured Movies -->
    <section class="featured-movies">
        <h2>Featured Movies</h2>
        <div class="movie-list">
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5pYTSJRCkoA4JfjNCpOwwbKp9YeltlRzioA&s" alt="Movie 1">
                <div class="movie-info">
                    <h3>Movie Title 1</h3>
                    <p>Rating: 8.5</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzuOTg-3hP_XwJ_LUh72E1WhwxgRQ4RMXVXA&s" alt="Movie 2">
                <div class="movie-info">
                    <h3>Movie Title 2</h3>
                    <p>Rating: 7.8</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="c:\Users\hi\Downloads\Telegram Desktop\photo_2025-01-16_05-27-23.jpg" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS4XjQL8zmNi-rJ3witxrRUhQtC8Eu_F0X5BQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7EFOMaYL_fI4uV_9AARMXcBPewcEgy-v1bw&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            

            
        </div>
    </section>

     <!-- Featured Movies -->
     <section class="featured-movies">
        <h2>Featured Movies</h2>
        <div class="movie-list">
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5pYTSJRCkoA4JfjNCpOwwbKp9YeltlRzioA&s" alt="Movie 1">
                <div class="movie-info">
                    <h3>Movie Title 1</h3>
                    <p>Rating: 8.5</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzuOTg-3hP_XwJ_LUh72E1WhwxgRQ4RMXVXA&s" alt="Movie 2">
                <div class="movie-info">
                    <h3>Movie Title 2</h3>
                    <p>Rating: 7.8</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>

            
        </div>
    </section>

      <!-- Featured Movies -->
      <section class="featured-movies">
        <h2>Featured Movies</h2>
        <div class="movie-list">
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5pYTSJRCkoA4JfjNCpOwwbKp9YeltlRzioA&s" alt="Movie 1">
                <div class="movie-info">
                    <h3>Movie Title 1</h3>
                    <p>Rating: 8.5</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzuOTg-3hP_XwJ_LUh72E1WhwxgRQ4RMXVXA&s" alt="Movie 2">
                <div class="movie-info">
                    <h3>Movie Title 2</h3>
                    <p>Rating: 7.8</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>

            
        </div>
    </section>

     <!-- Featured Movies -->
     <section class="featured-movies">
        <h2>Featured Movies</h2>
        <div class="movie-list">
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5pYTSJRCkoA4JfjNCpOwwbKp9YeltlRzioA&s" alt="Movie 1">
                <div class="movie-info">
                    <h3>Movie Title 1</h3>
                    <p>Rating: 8.5</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzuOTg-3hP_XwJ_LUh72E1WhwxgRQ4RMXVXA&s" alt="Movie 2">
                <div class="movie-info">
                    <h3>Movie Title 2</h3>
                    <p>Rating: 7.8</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>

            
        </div>
    </section>

     <!-- Featured Movies -->
     <section class="featured-movies">
        <h2>Featured Movies</h2>
        <div class="movie-list">
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5pYTSJRCkoA4JfjNCpOwwbKp9YeltlRzioA&s" alt="Movie 1">
                <div class="movie-info">
                    <h3>Movie Title 1</h3>
                    <p>Rating: 8.5</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzuOTg-3hP_XwJ_LUh72E1WhwxgRQ4RMXVXA&s" alt="Movie 2">
                <div class="movie-info">
                    <h3>Movie Title 2</h3>
                    <p>Rating: 7.8</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>

            
        </div>
    </section>
       <!-- Featured Movies -->
       <section class="featured-movies">
        <h2>Featured Movies</h2>
        <div class="movie-list">
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5pYTSJRCkoA4JfjNCpOwwbKp9YeltlRzioA&s" alt="Movie 1">
                <div class="movie-info">
                    <h3>Movie Title 1</h3>
                    <p>Rating: 8.5</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzuOTg-3hP_XwJ_LUh72E1WhwxgRQ4RMXVXA&s" alt="Movie 2">
                <div class="movie-info">
                    <h3>Movie Title 2</h3>
                    <p>Rating: 7.8</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>
            <div class="movie-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
                <div class="movie-info">
                    <h3>Movie Title 3</h3>
                    <p>Rating: 9.0</p>
                </div>
            </div>

            
        </div>
    </section>

   
   <!-- Featured Movies -->
   <section class="featured-movies">
    <h2>Featured Movies</h2>
    <div class="movie-list">
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5pYTSJRCkoA4JfjNCpOwwbKp9YeltlRzioA&s" alt="Movie 1">
            <div class="movie-info">
                <h3>Movie Title 1</h3>
                <p>Rating: 8.5</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzuOTg-3hP_XwJ_LUh72E1WhwxgRQ4RMXVXA&s" alt="Movie 2">
            <div class="movie-info">
                <h3>Movie Title 2</h3>
                <p>Rating: 7.8</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>

        
    </div>
</section>


   <!-- Featured Movies -->
   <section class="featured-movies">
    <h2>Featured Movies</h2>
    <div class="movie-list">
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5pYTSJRCkoA4JfjNCpOwwbKp9YeltlRzioA&s" alt="Movie 1">
            <div class="movie-info">
                <h3>Movie Title 1</h3>
                <p>Rating: 8.5</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzuOTg-3hP_XwJ_LUh72E1WhwxgRQ4RMXVXA&s" alt="Movie 2">
            <div class="movie-info">
                <h3>Movie Title 2</h3>
                <p>Rating: 7.8</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>
        <div class="movie-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxIl0vE09HM1flGc0EXYnG8h2OIylL5FsDzQ&s" alt="Movie 3">
            <div class="movie-info">
                <h3>Movie Title 3</h3>
                <p>Rating: 9.0</p>
            </div>
        </div>

        
    </div>
</section>



</marquee>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 FilmFlix, Inc. All rights reserved.</p>
    </footer>

    <script>
        // Search functionality
        document.getElementById("search-btn").addEventListener("click", function () {
            const searchQuery = document.getElementById("search").value.toLowerCase();
            const movieItems = document.querySelectorAll(".movie-item");

            movieItems.forEach(item => {
                const movieTitle = item.querySelector("h3").textContent.toLowerCase();
                if (movieTitle.includes(searchQuery)) {
                    item.style.display = "block"; // Show the item
                } else {
                    item.style.display = "none"; // Hide the item
                }
            });
        });

        // Button click events for the main banner (Play and My List)
        document.querySelectorAll(".main-banner button").forEach(button => {
            button.addEventListener("click", function () {
                const buttonText = button.textContent;
                if (buttonText === "Play") {
                    alert("Playing the movie...");
                } else if (buttonText === "My List") {
                    alert("Added to My List.");
                }
            });
        });
    </script>
</body>
</html>
