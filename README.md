# LIRI Bot

LIRI is like iPhone's SIRI. However, while SIRI is a Speech Interpretation and Recognition Interface, LIRI is a Language Interpretation and Recognition Interface. LIRI is a command line node app that takes in parameters and gives you back data.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install and how to install them

* [twitter](https://www.npmjs.com/package/twitter) - Twitter for Node.js
* [spotify](https://www.npmjs.com/package/node-spotify-api) - Spotify API Node.js
* [request](https://www.npmjs.com/package/request) - Request - Simplified HTTP client
* [dotenv](https://www.npmjs.com/package/dotenv) - Dotenv is a zero-dependency module that loads environment variables from a .env file into process.env

Installation instructions for each module can be found by following their links.

Obtain API keys for Twitter and Spotify.


### Installing

Clone or download the github repository.

```
git clone git@github.com:geekgirlbeta/liri-node-app.git
```

Install dotenv into the liri-node-app directory.

```
npm install dotenv --save
```
Make a .gitignore file and add the following lines to it.

```
node_modules
.DS_Store
.env
```

Create a file named .env, add the following to it, replacing the values with your API keys (no quotes) once you have them

```
# Spotify API keys

SPOTIFY_ID=your-spotify-id
SPOTIFY_SECRET=your-spotify-secret

# Twitter API keys

TWITTER_CONSUMER_KEY=your-twitter-consumer-key
TWITTER_CONSUMER_SECRET=your-twitter-consumer-secret
TWITTER_ACCESS_TOKEN_KEY=your-access-token-key
TWITTER_ACCESS_TOKEN_SECRET=your-twitter-access-token-secret

```

## Running the app from the command line.

```
node liri.js my-tweets

node liri.js spotify-this-song '<song name here>'

node liri.js movie-this '<movie name here>'

node liri.js do-what-it-says
```

These commands will log data into a log.txt file.

* `my-tweets`

* `spotify-this-song`

* `movie-this`

