# The-Entertainment-DataBase
This is a Simple Entertainment Information App built with Javascript using The Movie DataBase(TMDB) API.
(https://www.themoviedb.org/documentation/api) 

# Features
- The default page shows the list of Trending Movies.
- Lists Movies, TV Series, Anime, Cartoons, etc.
- Filter with Genre.
- Search by title.
- Page Navigation.
- Collection spans across the languages.
- View Summary of the Movie/Series/Anime along with trailers.

# Approach & Logic
The Data used in this project is fetched from themoviedb.org API(https://www.themoviedb.org/documentation/api).
**Structure of the Project:**
- index.html — contains the HTML layout which defines the element structure that would be shown on the page.
- style.css- contains CSS code for styling. Using CSS we can style the different portions to make them more visually appealing.
- script.js — contains Javascript code to fetch the API data and to represent it on browser.

**HTML Layout:**
Open VSCode and create the basic HTML structure in an index.html file by ! and then pressing tab. Give the title as ‘Movie App’. Link style.css and script.js to the created HTML file.Inside the body we will have header tag which contains h1 tag to display title of the app and form tag which holds the search bar used for searching the movies.we have div tag with the id content where our API fetched data will be presented dynamically.

**Javascript logic:**
Below functions are defined in the javascript code,
- getMovies() — A function to fetch movies from API and returns the results using fetch function.The results will be passed to showMovies() function.
- showMovies() — A function to showcase the results in the browser which basically inserts the HTML code dynamically.The data to this function is passed from the getMovies() function.
- setGenre() — A function to filter the content on the page with the genre selected by the user.
- clearBtn() — A function to clear the genre filters that are selected by the client to go back to the default page. 
- highlightSelection() — A function used to highlight the selected genre.
- An EventListener for search of movies.Once you enter the movie name in the search bar and by clicking on enter will actually submit the form and this event listerner will be triggered.The movie matching the name entered in the search bar will be fetched from the API and it will automatically display all the related title on the list.

**CSS Layout:**
Here we are arranging the list of the movies obtained from the API using flex . The img tag which holds image of the movie,the movie-info div class which holds information of the movie like movie name,the div class overview which has overview of the movie and knowmore which has the related teaser/trailer footage is inserted in the javascript code dynamically and not defined in the HTML file. The Page Navigation is located below with the arrows pointing to previous and next page.
Just hovering on the movie banner should actually show the overview. For that we are using transform: translateY(0);

# Deployment
This app is deployed using Netlify.
Link - https://entertainment-db.netlify.app/

# Further Improvements
This Website is built by HTML/CSS and Javascript. Using Frameworks like React, jQuery, etc. we can further improve this website by adding more categories like 'Now Playing', 'Alphabetical searching', 'Release Date order', 'Top Rated', etc.
