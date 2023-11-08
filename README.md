# Tinyurl
REST API web service written in Spring-Boot (Java), allows users to short URLs, monitor, track after them, and see statistics.

## Technologies
* Spring-Boot
* Docker
* JWT
* Databases:
  * MongoDB - Keeps track of user info and their related URL stuff, like the total clicks and how many clicks each URL gets.
  * Redis - Stores and maps short URLs to long URLs (key-value)
  * Cassandra - For storing and logging user's activity about URL visits (when, which URL, who visited)

## Features
* Short URL - The user can create a short URL for any URL
* URL Statistics - The user can see statistics about his URLs (total amount of clicks, total amount of clicks per URL, etc) via MongoDB
* URL Activity - The user can see activity about his URLs (when, which URL, who visited etc.) via Cassandra
