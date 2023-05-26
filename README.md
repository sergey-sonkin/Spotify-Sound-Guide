# Spotify-Recommendation-Engine

Spotify is currently criminally missing a feature to explore a new artist with the intention of finding a song of theirs to enjoy. Flipping through that artist's top tracks is not a practical alternative as many of the artist's top songs can be too similar to each other and Spotify's popularity metric arguably puts too much weight on recent releases.

The goal of this project is to simulate the experience of sitting with your best friend on the couch as they introduce you to their favorite artist. Your best friend on the couch would do anything to convince you that their favorite artist is the best. If you disliked a song, they would tell you that not all of the artist's songs are like that and would jump to a song that sounds different. With every song recommendation they'd be trying to win you over, using their infinite knowledge about every track by their favorite artist to curate each recommendation one after another.

Why doesn't Spotify do that? Not sure, but here's my attempt at doing just that using Spotify's own data.

Accomplished so far:
- Ingesting song features from Spotify API
- Transforming song features, dealing with duplicates and missing data, etc
- Defining metric for recommend ability of a song
- Suggesting songs by recommendability, prompting user for whether they enjoyed a song
- Cross referencing GeniusAPI for song lyrics for theme extraction with ChatGPT and embedding with BERT

In progress:
- A local PostGreSQL database to avoid duplicate lookups so we can scale userbase
- Rewrite from .ipynb to .py modules

In the future:
- Compelling seaborn visualizations to contextualize recommendations within discography
- A web-based frontend in Flask
