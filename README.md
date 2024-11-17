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

## Concepts
1. Show some rows
2. Think of the result set like a spreadsheet.
3. Adding columns.
4. Filtering: `WHERE`
5. Sorting: `ORDER BY` and `ORDER BY ... DESC`
6. Joining: `JOIN`
7. Aggregations: `SUM`, `COUNT`
8. Embedded queries, imagined tables
9. Sorting by aggregations

## Exercises
1. Look at films
2. Look at actors
2. What's the movie id for "academy dinosaur"?
3. Pick a film, show all the fields in the film table for that film
4. Show a full list of id, title, description for all films
5. Show the above for the last 10 films alphabetically.
6. Pick a film, show the full list of actors in it
7. Pick an actor, show their full list of films
8. From the list of films in #4, show how many actors are in it
9. Show the top 10 films by actor count in descending sequence
10. What are the possible rental durations for films?
11. Which rental durations are used most? Show the top 10 sorted descending with their counts
12. Show all the films with (some selected actor) and sort them by how many total actors were in the film.
13. Show a list of stores, who the manager is, the store address.
