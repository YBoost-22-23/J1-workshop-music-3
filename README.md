# workshop-music-3
YBoost workshop #3 | 12/10/2022

# Terminal Dataviz

## Objectif :
You have to create a golang program that will be able to display data visualization about music in the terminal.
You are free to choose the data you want to display but you can find in this link an example : https://www.instagram.com/rapminerz/
We recommand you tu use [termui](https://github.com/gizak/termui) to display your data.

## Notion :
* [Golang documentation : Flag](https://pkg.go.dev/flag)
* [Golang documentation : Os](https://pkg.go.dev/os)
* [Golang documentation : Termui](https://pkg.go.dev/github.com/gizak/termui/v3)
* [Retrive data from API in golang](https://tutorialedge.net/golang/consuming-restful-api-with-go/)

## Step 1 : Retrieve data
You have to retrieve data from API like : 
* [Shazam](https://rapidapi.com/apidojo/api/shazam)
* [Spotify](https://developer.spotify.com/documentation/web-api/)
* [Deezer](https://developers.deezer.com/api)
* [Last.fm](https://www.last.fm/api)
* [Genius](https://docs.genius.com/)
* [Musixmatch](https://developer.musixmatch.com/)
* [Soundcloud](https://developers.soundcloud.com/docs/api/guide)
* [Youtube](https://developers.google.com/youtube/v3)
* [Apple Music](https://developer.apple.com/documentation/applemusicapi)
* [Tidal](https://developers.tidal.com/)
* [Beatport](https://www.beatport.com/developer)
* [Discogs](https://www.discogs.com/developers/)

*Shazam API seems to be the easiest to use*  
Often, to use an API, you have to create an account and get an API key.
You are limited to a number of request per day. You can find the limit in the documentation of the API.

You can use [Postman](https://www.postman.com/) to test your API request.

## Step 2 : Display data
You have to display the data you retrieved in the terminal using [termui](https://pkg.go.dev/github.com/gizak/termui/v3)

## What is an API ?
An API is an interface that allows you to retrieve data from a website. API are set up by developers to allow other developers to use their data and make applications with it.

