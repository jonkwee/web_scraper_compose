# Web Scraper Docker Compose File

Docker compose file to create containers for my [selenium-web-scraper](https://github.com/jonkwee/selenium-web-scraper) project. 

## Containers
List of service containers involved in the compose file.

### MongoDB
MongoDB will be used as the primary data store for data scraped through [selenium-web-scraper](https://github.com/jonkwee/selenium-web-scraper). The compose file makes use of some environmental variables to set up the MongoDB container, so remember to set these up prior the creation of the containers.
* MONGODB_USER - username to access your mongodb service.
* MONGODB_PWD - password to access your mongodb service.
* MONGODB_DATA_PATH - path for docker to mount the `/data/db` so data can be persisted within the local context. (where your MongoDB will be storing your collection and data).

### MongoDB Express
Means to access your MongoDB through a web interface. The site can be accessed through `http://localhost:8081/`.