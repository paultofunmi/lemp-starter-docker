# Docker-PHP7

A quick and easy way to setup your PHP application using Docker and docker-compose. This will setup a developement environment with PHP7-fpm, MariaDB, Phpmyadmin and Nginx.

## Usage
~~~
git clone https://github.com/paultofunmi/lemp-starter-docker.git
cd lemp-starter-docker
docker-compose up
~~~

## Ports Information
~~~
Phpmyadmin: 8081
nginx: 8080
mariadb: 3306
~~~

### Structure

~~~
├── app
│   └── public
│       └── index.php
├── docker-compose.yml
├── storage
│   ├── database
│   └── logs
│        └── access.log
│        └── error.log
├── fpm
│   ├── Dockerfile
│   └── supervisord.conf
├── nginx
│   ├── Dockerfile
│   └── default.conf
~~~

- `app` is the directory for project files. Our Nginx config is pointing to `app/public`, which can be changed in `nginx/default.conf`
- `database` is where MariDB will store the database files.


### Credits 
shameerc @shameerc

