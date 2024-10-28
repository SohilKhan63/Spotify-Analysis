# Spotify Advanced SQL Project
Project Category: Advanced
[Click Here to get Dataset](https://www.kaggle.com/datasets/sanjanchaudhari/spotify-dataset)

![Spotify Logo]( https://www.freepik.com/search?format=search&last_filter=page&last_value=2&page=2&query=Spotify#uuid=c0f7a474-c808-4a38-a60d-950a47637620 )

## Overview
This project involves analyzing a Spotify dataset with various attributes about tracks, albums, and artists using **SQL**. It covers an end-to-end process of normalizing a denormalized dataset, performing SQL queries of varying complexity (easy, medium, and advanced), and optimizing query performance. The primary goals of the project are to practice advanced SQL skills and generate valuable insights from the dataset.

``` SQL
-- create table
DROP TABLE IF EXISTS spotify;
CREATE TABLE spotify 
	(
	Artist	VARCHAR(50),
	Track	VARCHAR(500),
	Album	VARCHAR(250),
	Album_type	VARCHAR(50),
	Danceability	FLOAT,
	Energy	FLOAT,
	Loudness	FLOAT,
	Speechiness	FLOAT,
	Acousticness	FLOAT,
	Instrumentalness	FLOAT,
	Liveness	FLOAT,
	Valence	FLOAT,
	Tempo	FLOAT,
	Duration_min	FLOAT,
	Title	VARCHAR(500),
	Channel	VARCHAR(100),
	Views	BIGINT,
	Likes	BIGINT,
	Comments	BIGINT,
	Licensed	BIGINT,
	official_video	BOOLEAN,
	Stream	BIGINT,
	EnergyLiveness	FLOAT,
	most_playedon	VARCHAR(100) 
	);

```
## Project Steps

### 1. Data Exploration
Before diving into SQL, it’s important to understand the dataset thoroughly. The dataset contains attributes such as:
- `Artist`: The performer of the track.
- `Track`: The name of the song.
- `Album`: The album to which the track belongs.
- `Album_type`: The type of album (e.g., single or album).
- Various metrics such as `danceability`, `energy`, `loudness`, `tempo`, and more.


#### Easy Queries
- Simple data retrieval, filtering, and basic aggregations.
  
#### Medium Queries
- More complex queries involving grouping, aggregation functions, and joins.
  
#### Advanced Queries
- Nested subqueries, window functions, CTEs
---

## 13 Practice Questions

### Easy Level
1. Retrieve the names of all tracks that have more than 1 billion streams.
2. List all albums along with their respective artists.
3. Get the total number of comments for tracks where `licensed = TRUE`.
4. Find all tracks that belong to the album type `single`.
5. Count the total number of tracks by each artist.

### Medium Level
1. Calculate the average danceability of tracks in each album.
2. Find the top 5 tracks with the highest energy values.
3. List all tracks along with their views and likes where `official_video = TRUE`.
4. For each album, calculate the total views of all associated tracks.
5. Retrieve the track names that have been streamed on Spotify more than YouTube.

### Advanced Level
1. Find the top 3 most-viewed tracks for each artist using window functions.
2. Write a query to find tracks where the liveness score is above the average.
3. **Use a `WITH` clause to calculate the difference between the highest and lowest energy values for tracks in each album.**



Here’s an updated section for your **Spotify Advanced SQL Project and Query Optimization** README, focusing on the query optimization task you performed. You can include the specific screenshots and graphs as described.

---


## Technology Stack
- **Database**: PostgreSQL
- **SQL Queries**: DDL, DML, Aggregations, Joins, Subqueries, Window Functions, CTEs
- **Tools**: pgAdmin 4 (or any SQL editor)

## How to Run the Project
1. Install PostgreSQL and pgAdmin (if not already installed).
2. Set up the database schema and tables using the provided normalization structure.
3. Insert the sample data into the respective tables.
4. Execute SQL queries to solve the listed problems.
5. Explore query optimization techniques for large datasets.

---

## Contributing
If you would like to contribute to this project, feel free to fork the repository, submit pull requests, or raise issues.

