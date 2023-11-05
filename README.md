# Tinyurl
REST API web service written in Spring-Boot (Java), allows users to short URLs, monitor, track after them, and see statistics.

## Technologies
* Spring-Boot
* Docker
* JWT
* Databases:
  * MongoDB - for storing users and URLS data related to them (total amount of clicks, total amount of clicks per url, etc)
  * Redis - for storing and mapping short URL to long URL (key-value)
  * Cassandra - for storing and logging user's activity about URL visits (when, which URL, who visited etc.)
