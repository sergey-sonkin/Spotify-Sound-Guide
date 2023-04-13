# Spotify-Artist-Guide

The goal of this project is to simulate the experience of sitting with your best friend on the couch as they introduce you to their favorite artist.

Spotify is currently criminally missing a feature to explore a new artist with the intention of finding a song of theirs to enjoy. Flipping through that artist's top tracks is not a practical alternative as many of the artist's top songs can be too similar to each other and Spotify's popularity metric arguably puts too much weight on recent releases.

Your best friend on the couch would do anything to convince you that their favorite artist is the best. If you disliked a song, they would tell you that not all of the artist's songs are like that and would jump to a different sounding song. With every song recommendation they'd be trying to win you over, using their infinite knowledge about every track by their favorite artist to curate each recommendation one after another.

Why doesn't Spotify do that? Not sure, but here's my attempt at doing just that using Spotify's own data.

Accomplished so far:
- Ingesting song features from Spotify API
- Transforming song features, dealing with duplicates and missing data, etc
- Defining metric for recommendability of a song
- Suggesting songs by recommendability, prompting user for whether they enjoyed a song

In progress:
- An alternative to Spotify's missing popularity metric 
- Additional song filtering (i.e interludes) to avoid "bad" suggestions
- A web-based frontend in Flask with the help of ChatGPT4

Goals down the road:
- Creating a local PostGreSQL database to avoid duplicate lookups if we ever scale userbase
- Additional metadata: cross referencing YTMusicAPI or AppleMusicAPI for lyric and genre data
- NLP on aforementioned lyric data
