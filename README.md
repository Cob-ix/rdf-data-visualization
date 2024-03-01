# Spotify Songs and Playlists Analysis Project

## Overview
This project provides an analytical view of 30,000 songs extracted from Spotify playlists, highlighting album releases, genre distributions, and artist popularity trends.

## Features
- Visualization of album releases over the years.
- Genre analysis displaying the count of tracks per genre.
- Artist popularity tracking over time.
- Interactive elements to filter data based on genres and artists.
- Average age of the artists at their first album release (currently not working) 

## Dataset Source
The data is based on a [Kaggle dataset](https://www.kaggle.com/datasets/joebeachcapital/30000-spotify-songs) of 30,000 Spotify songs.

## How to Use
1. **Album Release Trends**: View the graph showing the distribution of album releases over the years.
2. **Genre Analysis**: Explore the graph detailing the number of tracks per genre.
3. **Artist Popularity**: Search for artists to visualize their track popularity across different years.
4. **Danceability and Speechiness**: Compare these metrics across selected genres.

## Technical Details
- Employs `d3sparql.js` for querying, handling SPARQL results and data visualization.
- Integrates with a SPARQL endpoint to fetch data.

## Installation & execution

You need docker compose to build this project.
To build the project, execute the following commands:

> Note: Building the images can take a few minutes.

```bash
docker-compose build --no-cache fuseki
docker-compose build --no-cache d3_webserver
```

Then to start the project, execute :

```bash
docker compose up
```

The Fuseki web UI will be accessible on `localhost:3030` and the web app for data visualization will be accessible on `localhost:8080`.
The fuseki database endpoint is on `localhost:3333`.