-----------------------------------------------------------------------
Return ALL the data in the 'movies' table.

SELECT * FROM movies;

-----------------------------------------------------------------------
Return ONLY the name column from the 'people' table

SELECT people.name FROM people;

----------------------------------------------------------------------
Oops! Someone at CodeClan spelled Keith's name wrong! Change it to reflect the proper spelling.

UPDATE people
SET name = 'Keith Douglas'
WHERE id = 22;

-----------------------------------------------------------------------
Return ONLY your name from the 'people' table.

SELECT people.name
FROM people
WHERE id = 20;

-----------------------------------------------------------------------
The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.

DELETE FROM movies
WHERE title = 'Batman Begins';

SELECT * FROM movies;  Purely to verify it was deleted

-----------------------------------------------------------------------
Create a new entry in the 'people' table with the name of one of the instructors.

INSERT INTO people (name) VALUES('John Harper')

-----------------------------------------------------------------------
Pawel has decided to hijack our movie evening, Remove him from the table of people.

He already gone!
So add him first then delete him!

INSERT INTO people (name) VALUES('Pawel Johnson');
SELECT * FROM people;

DELETE FROM people
WHERE id = 23

-----------------------------------------------------------------------
The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this.

INSERT INTO movies (title, year, show_time) VALUES ('Avengers: Infinity War', 2018, '00:00');

-----------------------------------------------------------------------
The cinema would also like to make the Guardians movies a back to back feature. Find out the show time of "Guardians of the Galaxy" and set the show time of "Guardians of the Galaxy 2" to start two hours later.

SELECT * FROM movies; Find the show time of guardians and the index of guardians 2

UPDATE movies
SET show_time = '18:20' update guardians 2 showtime
WHERE id = 16;

SELECT * FROM movies; check update has happened

-----------------------------------------------------------------------

Extension

Delete multiple entries from your table in a single command.

DELETE FROM movies
WHERE year = 2011;  deleting all movies from 2011
SELECT * FROM movies;

----------------------------------------------------------------------
Select all the movies ordered by year in descending order

SELECT * FROM movies
ORDER BY year ASC;

----------------------------------------------------------------------
