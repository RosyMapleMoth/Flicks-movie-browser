# Flix
Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

### User Stories

- [x] User can view a list of movies (title, poster image, and overview) currently playing in theaters from the Movie Database API.
- [x] Views should be responsive for both landscape/portrait mode.
   - [x] In portrait mode, the poster image, title, and movie overview is shown.
   - [x] In landscape mode, the rotated alternate layout should use the backdrop image instead and show the title and movie overview to the right of it.
- [x] Display a nice default [placeholder graphic](https://guides.codepath.com/android/Displaying-Images-with-the-Glide-Library#advanced-usage) for each image during loading
- [x] Improved the user interface by experimenting with styling and coloring.
- [x] Expose details of movie (ratings using RatingBar, popularity, and synopsis) in a separate activity.
- [x] Allow video posts to be played in full-screen using the YouTubePlayerView.
- [x] Trailers for popular movies are played automatically when the movie is selected
  - [x] When clicking on a popular movie (i.e. a movie voted for more than 5 stars) the video should be played immediately.
  - [x] Less popular videos rely on the detailed page should show an image preview that can initiate playing a YouTube video. 
- [x] Add a rounded corners for the images using the Glide transformations. 
- [x] added genre infermation for each movie by calling the TMDB api again to find the list of all genres based on genre code.

### App Walkthough GIF
First pass,<br>
<img src="https://i.imgur.com/R80KFhG.gif" width=250><br>
current build.<br>
<img src="https://i.imgur.com/WoiBdz0.gif" width=250><br>

### Notes
I had a great deal of trouble with the [Android Async HTTP] and Glide at first but now i understand at least the basics of their use. Mainly my issues stemmed from not using the debugger to step through large issues 

edit : by far the hardest thing was adding genre information

### Open-source libraries used

- [Android Async HTTP](https://github.com/loopj/android-async-http) - Simple asynchronous HTTP requests with JSON parsing
- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Androids
