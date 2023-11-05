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
