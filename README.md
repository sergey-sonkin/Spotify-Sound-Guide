# Spotify-Artist-Guide

The goal of this project is to simulate the experience of sitting with your best friend on the couch as they introduce you to their favorite artist.

Spotify is currently criminally missing a feature to explore a new artist with the intention of finding a song of theirs to enjoy. Flipping through an artist's top tracks is not an alternative as many of the artist's top songs can be too similar to each other and Spotify's popularity metric arguably puts too much weight on recent releases.

Accomplished so far:
- Ingesting song features from Spotify API
- Transforming song features, dealing with duplicates and missing data, etc
- Defining metric for recommendability of a song
- Suggesting songs by recommendability, prompting user for whether they enjoyed a song

In progress:
- An alternative to Spotify's missing popularity metric 
- Additional song filtering (i.e interludes) to avoid "bad" suggestions
- Storing song information in a local PostGreSQL database to avoid duplicate lookups

Goals down the road:
- Additional metadata: cross referencing YTMusicAPI or AppleMusicAPI for lyric and genre data
- NLP on aforementioned lyric data
- Adding a web-based frontend with Flask with the help of ChatGPT4 (I've never developed a front end before)
