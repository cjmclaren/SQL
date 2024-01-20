# This analysis uses three tables that I created using information from IMDB.com.

# Create a table with actors' personal information
CREATE TABLE actors (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    first_name TEXT,
    last_name TEXT,
    birthyear INTEGER,
    gender TEXT,
    spouse_id INTEGER);
    
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Blake", "Lively", "1987", "female", "4");
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Harrison", "Ford", "1942", "male", "3");
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Calista", "Flockhart", "1964", "female", "2");
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Ryan", "Reynolds", "1976", "male", "1");
INSERT INTO actors (first_name, last_name, birthyear, gender) VALUES ("Henry", "Cavill", "1983", "male");
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Melissa", "Benoist", "1988", "female", "7");
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Chris", "Wood", "1988", "male", "6");
INSERT INTO actors (first_name, last_name, birthyear, gender) VALUES ("Ezra", "Miller", "1992", "male");
INSERT INTO actors (first_name, last_name, birthyear, gender) VALUES ("Emma", "Watson", "1990", "female");
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Sean", "Astin", "1971", "male", "11");
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Christine", "Astin", "1967", "female", "10");
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Jim", "Parsons", "1973", "male", "13");
INSERT INTO actors (first_name, last_name, birthyear, gender, spouse_id) VALUES ("Todd", "Spiewak", "1977", "male", "12");
INSERT INTO actors (first_name, last_name, birthyear, gender) VALUES ("Kaley", "Cuoco", "1985", "female");


# Create a table about movies, movie characters, and the id numbers of actors who play them
CREATE TABLE movies (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    category TEXT,
    movie_title TEXT,
    character_name TEXT,
    actor_id INTEGER);
    
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("drama", "The Age of Adaline", "Adaline Bowman", "1");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("drama", "The Age of Adaline", "William Jones", "2");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("superheroes", "Man of Steel", "Superman", "5");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("adventure", "Indiana Jones and the Last Crusade", "Indiana Jones", "2");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("superheroes", "Green Lantern", "Hal Jordan", "4");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("superheroes", "Justice League", "The Flash", "8");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("superheroes", "Batman vs Superman", "Superman", "5");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("adventure", "Fantastic Beasts and Where to Find Them", "Credence Barebone", "8");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("drama", "The Proposal", "Andrew Paxton", "4");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("superheroes", "Green Lantern", "Carol Ferris", "1");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("drama", "The Perks of Being a Wallflower", "Patrick", "8");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("drama", "The Perks of Being a Wallflower", "Sam", "9");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("adventure", "The Goonies", "Mikey", "10");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("adventure", "The Fellowship of the Ring", "Sam", "10");
INSERT INTO movies (category, movie_title, character_name, actor_id) VALUES ("adventure", "Home", "Oh", "12");

# Create a table about tv shows, tv show characters, and the id numbers of actors who play them
CREATE TABLE tv_shows (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    category TEXT,
    show_title TEXT,
    character_name TEXT,
    actor_id INTEGER);
    
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("superheroes", "Supergirl", "Supergirl", "3");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("superheroes", "Supergirl", "Mon-El", "7");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("superheroes", "The Flash", "Supergirl", "3");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("superheroes", "The Flash", "Mon-El", "7");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("superheroes", "The Flash", "The Flash", "8");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("superheroes", "Supergirl", "Cat Grant", "3");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("drama", "Gossip Girl", "Serena van der Woodsen", "1");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("drama", "Shrinking", "Paul", "2");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("drama", "The Tudors", "Charles Brandon", "5");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("superheroes", "Supergirl", "Pete Andrews", "10");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("drama", "Stranger Things", "Bob Newby", "10");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("drama", "The Big Bang Theory", "Dr. Greg Pemberton", "10");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("drama", "The Big Bang Theory", "Sheldon Cooper", "12");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("drama", "The Big Bang Theory", "Penny", "14");
INSERT INTO tv_shows (category, show_title, character_name, actor_id) VALUES ("adventure", "Harley Quinn", "Harley Quinn", "14");


# Show all data from all three tables
SELECT *
FROM actors;

SELECT *
FROM movies;

SELECT *
FROM tv_shows;

# Write a query showing the actors who are married next to the name of their spouses
SELECT a.first_name, a.last_name,
  b.first_name || ' ' || b.last_name AS "spouse"
FROM actors AS a
INNER JOIN actors AS b
ON a.spouse_id = b.id;

# Which actors are not married?
SELECT first_name, last_name
FROM actors
WHERE spouse_ID IS NULL;

# Which movies and tv shows has Ezra Miller been in?
SELECT movies.movie_title,
    tv_shows.show_title
FROM actors AS a
LEFT JOIN movies ON a.id = movies.actor_id
LEFT JOIN tv_shows ON a.id = tv_shows.actor_id
WHERE a.first_name = "Ezra"
    AND a.last_name = "Miller";

# How many superhero movies are there?
SELECT COUNT(DISTINCT movie_title) AS "Number of Superhero Movies"
FROM movies
WHERE category = "superheroes";

# Who acted in The Age of Adaline?
SELECT m.movie_title, a.first_name, a.last_name
FROM movies AS m
JOIN actors AS a ON m.actor_id = a.id
WHERE m.movie_title = "The Age of Adaline";

# Add a category classifying the age group of each actor and order the results from youungest to oldest.
SELECT *,
	CASE
    	WHEN birthyear <= 1959 THEN "senior citizen"
        WHEN birthyear <= 1984 THEN "over the hill"
        ELSE "younger generation"
	END AS "age category"
FROM actors
ORDER BY birthyear desc;

# How many actors are there of each gender?
SELECT gender, COUNT(*) AS number
FROM actors
GROUP BY gender;

# What is the average age of actors?
SELECT ROUND(AVG(CURRENT_DATE - birthyear),1) AS average_age
FROM actors;
