# liri-node-app

Homework from Michael Rodriguez


# LIRI Bot
### LIRI is like iPhone's SIRI, however, while SIRI is a Speech Interpretation and Recognition Interface,
### LIRI is a Language Interpretation and Recognition Interface. 
### LIRI is a command line node app that takes in on of four parameters and returns the relative data.
`` spotify-this-song ``
`` movie-this ``
`` concert-this ``
`` do-what-it-says ``

1. Deployment
2. Clone repo
3. Run npm install
4. At command prompt run node liri.js <pass in an instruction from above>
5. Screenshot of this Project
6. Liri Bot

## The syntax to run the program is:
### node liri.js spotify-this-song "name a song"

* ## Logs the following information:
* artist(s)
* song name
* preview link of the song from spotify
* album
* if no song is provided then the program will output information for the song "What's my age again?" by Blink 182

## The syntax to run the program is:
### node liri.js movie-this "enter movie title"

 ## Logs the following information:
* Title
* Year
* IMDB Rating
* Country
* Language
* Plot
* Actors
* Rotten Tomatoes Rating
* Rotten Tomatoes URL
* if no movie is provided then the program will output information for the movie "The Secret Window" with Johnny Depp

## The syntax to run the program is:
### node liri.js concert-this "enter artist name"

## Logs the following information:
* Artist's name
* APP_ID
* Event List
* Dates (yyy-mm-dd)

* ### The program will take the text inside of random.txt and use it to call the first command with the second part as it's parameter
* ### Currently in random.txt, the following text is there:
`` spotify-this-song, "Sunday Best" ``

# Technologies Utilized
* NodeJS
* JavaScript
* Spotify API
* Bands in Town API
* OMDB API
* NPM installer
* NPM spotify-web-api-node
* NPM dotenv
* NPM request


  ## Installation

To run the application locally, first clone this repository with the following command:

	git clone https://github.com/mriguez777/liri-node-app.git
	
Next, install the application dependencies.

    npm init
	npm install

    *You will need to create a keys.js file and fill in the following code: inside the "//". You will need to gather your own API keys for Spotify (https://developer.spotify.com/documentation/web-api/), OMDB (http://www.omdbapi.com/) and bandsInTown (https://www.artists.bandsintown.com/support/api-installation). 

    
    //
exports.spotify = {
  id: "",
  secret: ""
};
exports.bandsInTownAPI = {
  id: ""
};
exports.omdb = {
  id: ""
}
//
	
Finally, run the node server locally. Please note with where it says "enter a song", "artist name" an "movie title", enter in one of your choice as it can search for all three or one at a time. 

	node liri.js `spotify-this-song "enter in a song"`, 
    node liri.js `concert-this "artist name"`,
    node liri.js `movie-this "movie title" 
    node liri.js 'do-what-it-says'


## Working code images in the repo 
spotify-working.png
movie-working.png
