# liri-node-app

<p>LIRI is like iPhone's SIRI. However, while SIRI is a Speech Interpretation and Recognition Interface, LIRI is a Language Interpretation and Recognition Interface. LIRI will be a command line node app that takes in parameters and gives you back data.</p>

<h2>Geting started</h2>
<ol>
<li>Clone the repository on your local machine.</li>
<li>2.Open the terminal in the correct folder and run npm install to install all the dependencies</li>
   <ul>
      <li>Node-Spotify-API</li>
      <li>Request</li>
      <li>Moment</li>
      <li>DotEnv</li>
      <li>console.table</li>
   </ul>
<li>get a spotify-key.</li>
</ol>
<h3>What Each Command Should Do</h3>

1.node liri.js concert-this <artist/band name here>

<li>This will search the Bands in Town Artist Events API ("https://rest.bandsintown.com/artists/" + artist + "/events?app_id=**********") for an artist and render the following information about each event to the terminal:</li>
<ul>
<li>Name of the venue</li>
<li>Venue location</li>
<li>Date of the Event (use moment to format this as "MM/DD/YYYY")</li>
</ul>
2.node liri.js spotify-this-song '<song name here>'

<li>This will show the following information about the song in your terminal/bash window</li>
<ul>
<li>Artist(s)</li>
<li>The song's name</li>
<li>A preview link of the song from Spotify</li>
<li>The album that the song is from</li>
</ul>

<li>If no song is provided then your program will default to "I Want it That Way" by ...</li>
<li>You will utilize the<a href ="https://www.npmjs.com/package/node-spotify-api" target = "_blank">node-spotify-api</a> package in order to retrieve song information from the Spotify API.</li>
<li>The Spotify API requires you sign up as a developer to generate the necessary credentials. You can follow these steps in order to generate a <strong>client id</strong> and <strong>client secret:</strong></li>
<li>Step One: Visit <a href="https://developer.spotify.com/my-applications/#!/" target = "_blank">https://developer.spotify.com/my-applications/#!/</a></li>
<li>Step Two: Either login to your existing Spotify account or create a new one (a free account is fine) and log in.</li>
<li>Step Three: Once logged in, navigate to <a href = "https://developer.spotify.com/my-applications/#!/applications/create target = "_blank">https://developer.spotify.com/my-applications/#!/applications/create </a> to register a new application to be used with the Spotify API. You can fill in whatever you'd like for these fields. When finished, click the "complete" button.</li> finished, click the "complete" button.
<li>Step Four: On the next screen, scroll down to where you see your client id and client secret. Copy these values down somewhere, you'll need them to use the Spotify API and the <a href ="https://www.npmjs.com/package/node-spotify-api" target = "_blank">node-spotify-api package</a>.</li>

3.node liri.js movie-this '<movie name here>'

This will output the following information to your terminal/bash window:
<ul>
   <li>* Title of the movie.</li>
   <li>* Year the movie came out.</li>
   <li>*IMDB Rating of the movie.</li>
   <li>* Rotten Tomatoes Rating of the movie.</li>
   <li>* Country where the movie was produced.</li>
   <li>* Language of the movie.</li>
   <li>* Plot of the movie.</li>
   <li>* Actors in the movie.</li>
</ul>
<li>If the user doesn't type a movie in, the program will output data for the movie 'Mr. Nobody.'</li>
<ul>
<li>If you haven't watched "Mr. Nobody," then you should: <a href="http://www.imdb.com/title/tt0485947/"> http://www.imdb.com/title/tt0485947/</a></li>

<li>It's on Netflix!</li>
</ul>

<li>You'll use the request package to retrieve data from the OMDB API. The OMDB API requires an API key.</li>

4.node liri.js do-what-it-says

<li>Using the fs Node package, LIRI will take the text inside of random.txt and then use it to call one of LIRI's commands.</li>
<ul>
<li>It should run spotify-this-song for "I Want it That Way," as follows the text in random.txt.</li>
<li>Edit the text in random.txt to test out the feature for movie-this and concert-this</li>
</ul>
<h2>Built With</h2>
<p>JavasScript, Bands in Town API, Spotify API, OMDB API.</p>








