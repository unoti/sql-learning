

```sql
SELECT * FROM actor;
SELECT * FROM actor LIMIT 5;
SELECT actor_id, last_name, first_name FROM actor LIMIT 10;

SELECT film_id, title, rental_duration
FROM film
WHERE rental_duration == 4;

SELECT film_id, title, rental_duration
FROM film
WHERE title LIKE '%RACE%';

SELECT film_id, title, rental_duration
FROM film
ORDER BY film_id DESC; -- can leave blank for ascending, or use ASC

SELECT film_id, title, rental_duration
FROM film
WHERE title LIKE 'alabam%'

SELECT f.film_id
, f.title
, fa.actor_id
FROM film f
JOIN film_actor fa ON f.film_id = fa.film_id
WHERE f.title LIKE 'ALAB%'

SELECT actor_id, first_name, last_name
FROM actor
WHERE actor_id IN (1,10,20,30,40,53,108,162,188,198)

-- All the actors that appeared in film id 1
SELECT fa.actor_id
, fa.film_id
, f.title
, a.first_name
, a.last_name
FROM film_actor fa
JOIN film f ON fa.film_id = f.film_id
JOIN actor a ON fa.actor_id = a.actor_id
WHERE f.film_id = 1

-- Everyone that appeared in a film searching by name.
SELECT fa.actor_id
, fa.film_id
, f.title
, a.first_name
, a.last_name
FROM film_actor fa
JOIN film f ON fa.film_id = f.film_id
JOIN actor a ON fa.actor_id = a.actor_id
WHERE f.title LIKE '%ACADEMY DINO%'
ORDER BY f.title

```