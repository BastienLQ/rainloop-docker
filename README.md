# Docker images for Rainloop

## Building

````bash
docker build -t "bastien/rainloop:community" community/
````

````bash
docker build -t "bastien/rainloop:standard" standard/
````

## Running

````bash
docker run -it -d --restart=always --publish 127.0.0.1:80:80 bastien/rainloop:community
````

Additionally, you can map volume `/var/www/html/data`.
