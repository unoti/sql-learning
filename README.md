# SQL Learning

Started this to show someone the basics of SQL.

## Resources
* Got this from [sakila-sqlite3 on Github](https://github.com/bradleygrant/sakila-sqlite3?tab=readme-ov-file)
* [SQLlite Cheat Sheet](https://www.sqlitetutorial.net/sqlite-commands/)

## Installing
Try running the `sqlite3` command below in Ubuntu, and ubuntu will tell you how to install it.

## Running
```bash
$ sqlite3 sakila_master.db
```

## Commands
```sql
.tables
.schema table_name
```

## Intro
1. How to look at a couple of tables here, films and actors
2. How to use LIMIT to show just a few records.
3. How to read a schema diagram.

![Schema Diagram](docs/sakila.png)

## Exercises
1. Look at films
2. Look at actors
3. Pick a film, show everything about it
4. Show a full list of id, title, description for all films
5. Show the above for the top 10 films alphabetically.
6. Pick a film, show the full list of actors in it
7. Pick an actor, show their full list of films
8. From the list of films in #4, show how many actors are in it
9. Show the top 10 films by actor count in descending sequence
10. Show all the films with (some selected actor) and sort them by how many total actors were in the film.
