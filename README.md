Download Link: https://assignmentchef.com/product/solved-comp3311-assignment-3
<br>



## Goal:This assignment aims to give practice in

– manipulating a moderately large database (IMDB)– implementing SQL views to satisfy requests for information– implementing PLpgSQL functions to satisfy requests for information– implementing Python scripts to extract and display data

The goal is to build some useful data access operations on the Internet Movie Database (IMDB), which contains a wealth of information about movies, actors, etc. You need to write Python scripts, using the Psycopg2 database connectivity module, to extract and display information from this database.

### Introduction

The Internet Movie Database (IMDB) is a huge collection ofinformation about all kinds of video media.It has data about most movies since the dawn of cinema, butalso a vast amount of information about TV series, documentaries,short films, etc.Similarly, it holds information about the people who workedon and starred in these video artefacts.It also hold viewer ratings and crticis reviews for video artefactsas well as a host of other trivia (e.g. bloopers).

The full IMDB database is way too large to let you all build copiesof it, so we have have created a cut-down version of thedatabase that deals with well-rated movies from the last 60 years.You can find more details on the database schema inhttps://cgi.cse.unsw.edu.au/~cs3311/20T3/assignments/ass3/database.php

the data only goes to mid 2019, so you won’t find recent blockbusters.

### Questions

Q1

– Complete the script called “best” so that it printsa list of the top N highest-rating movies (default N = 10).The script takes a single command-line argument which specifies howmany movies should appear in the list.Movies should be ordered from highest to lowest rating, and shouldbe displayed as, e.g.

Q2

– Complete the script called “rels” so that it printsa list of the different releases (different regions, differentlanguages) for a movie.The script takes a single command-line argument which givesa part of a movie name (could be the entire name).If there are no movies matching the supplied partial-name,then you should print a message to this effect and quit theprogram

Q3– Complete the script called “minfo” so that it printsa list of cast and crew for a movie.The script takes a command-line argument which givesa part of a movie name (could be the entire name).It also takes an optional command-line argument, whichis a year and can be used to distinguish movies withthe same title (or, at least, titles which match thepartial movie name).

Q4

– Complete the script called “bio” so that it printsa filmography for a given person (Name), showingtheir roles in each of the movies they are associated with.The script takes a command-line argument which givesa part of a person’s name (could be the entire name).It also takes an optional command-line argument, whichis a year (their birth year) and which can be used todistinguish people with similar names.


