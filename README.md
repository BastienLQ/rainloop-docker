# Docker images for Rainloop

## Building

````bash
cd community/
docker build -t "rainloop-community:latest" .
````

````bash
cd standard/
docker build -t "rainloop-standard:latest" .
````

## Running

````bash
docker run -it -d --restart=always --publish 127.0.0.1:80:80 rainloop-community
````

Additionally, you can map volume `/var/www/html/data`.
