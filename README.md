# Nordic Thingy with Spotify

ID2012 Ubiquitous Computing Project where we use Nordic Thingy to control Spotify playback:

1. Right tilt to skip to next track
2. Left tilt to skip to previous track
3. Put Thingy down to pause the track
4. Stand Thingy up to play the track

Thingy also gives visual cues when changing the playback. The LED blinks when tracks are skipped. When the playback stops, LED switches to red colour, and it emits green light when playback starts.


## Installation

These examples run on Node.js. On [its website](http://www.nodejs.org/download/) you can find instructions on how to install it. You can also follow [this gist](https://gist.github.com/isaacs/579814) for a quick and easy way to install Node.js and npm.

Once installed, clone the repository and install its dependencies running:

    $ npm install

### Using your own credentials
You will need to register your app and get your own credentials from the Spotify for Developers Dashboard.

To do so, go to [your Spotify for Developers Dashboard](https://beta.developer.spotify.com/dashboard) and create your application. For the examples, we registered these Redirect URIs:

* http://localhost:8888 (needed for the implicit grant flow)
* http://localhost:8888/callback

Once you have created your app, replace the `client_id`, `redirect_uri` and `client_secret` in the examples with the ones you get from My Applications.

## Running the Project
In order to run the project, run its `app.js` file. 
    $ node app.js

Then, open `http://localhost:8888` in a browser.
