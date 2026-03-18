# BoltSql_Monali
**Exercise 1 — Tasks**
Find the title of each film 
(SELECT title FROM movies;)
Find the director of each film 
(SELECT director FROM movies;)
Find the title and director of each film 
(SELECT title, director FROM movies;)
Find the title and year of each film 
(SELECT title, year FROM movies;)
Find all the information about each film 
(SELECT * FROM movies;)

**Exercise 2 — Tasks**
Find the movie with a row id of 6 
(SELECT * FROM movies where id = 6;)
Find the movies released in the years between 2000 and 2010
(SELECT title FROM movies where year > 2000 and year < 2010;)
Find the movies not released in the years between 2000 and 2010
(SELECT title FROM movies where year < 2000 or year > 2010;)
Find the first 5 Pixar movies and their release year
(SELECT title FROM movies where id < 6;)

**Exercise 3 — Tasks**
1. Find all the Toy Story movies
(SELECT * FROM movies where title like "Toy Story%";)
2. Find all the movies directed by John Lasseter
(SELECT * FROM movies where director like "John Lasseter";)
3. Find all the movies (and director) not directed by John Lasseter
(SELECT * FROM movies where director not like "John Lasseter";)
4. Find all the WALL-* movies
(SELECT * FROM movies where title like "Wall-%";)

**Exercise 4 — Tasks**
1. List all directors of Pixar movies (alphabetically), without duplicates
(SELECT distinct(director) from movies order by director asc;)
2. List the last four Pixar movies released (ordered from most recent to least)
(SELECT title FROM movies order by year desc limit 4;)   
3. List the first five Pixar movies sorted alphabetically
(SELECT title FROM movies
ORDER BY title ASC
LIMIT 5;)
4. List the next five Pixar movies sorted alphabetically
(SELECT title FROM movies
ORDER BY title ASC
LIMIT 5 OFFSET 5;)

**EXERCISE 5 — Tasks**
1. List all the Canadian cities and their populations
(SELECT city, population FROM north_american_cities
WHERE country = "Canada";)
2. Order all the cities in the United States by their latitude from north to south
(SELECT city, latitude FROM north_american_cities
WHERE country = "United States"
ORDER BY latitude DESC;)
3. List all the cities west of Chicago, ordered from west to east
(SELECT city, longitude FROM north_american_cities
WHERE longitude < -87.629798
ORDER BY longitude ASC;)
4. List the two largest cities in Mexico (by population)
(SELECT city, population FROM north_american_cities
WHERE country LIKE "Mexico"
ORDER BY population DESC
LIMIT 2;)
5. List the third and fourth largest cities (by population) in the United States and their population
(SELECT city, population FROM north_american_cities
WHERE country LIKE "Mexico"
ORDER BY population DESC
LIMIT 2;)
