# BoltSql_Monali
**Exercise 1 — Tasks**
Find the title of each film 
SELECT title FROM movies;
Find the director of each film 
SELECT director FROM movies;
Find the title and director of each film 
SELECT title, director FROM movies;
Find the title and year of each film 
SELECT title, year FROM movies;
Find all the information about each film 
SELECT * FROM movies;

**Exercise 2 — Tasks**
Find the movie with a row id of 6 
SELECT * FROM movies where id = 6;
Find the movies released in the years between 2000 and 2010
SELECT title FROM movies where year > 2000 and year < 2010;
Find the movies not released in the years between 2000 and 2010
SELECT title FROM movies where year < 2000 or year > 2010;
Find the first 5 Pixar movies and their release year
SELECT title FROM movies where id < 6;

**Exercise 3 — Tasks**
Find all the Toy Story movies
Find all the movies directed by John Lasseter
Find all the movies (and director) not directed by John Lasseter
Find all the WALL-* movies
