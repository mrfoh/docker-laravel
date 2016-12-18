# Laravel applications with Docker
This repo contains a Laravel installation setup to use Docker to create a development environment. This repo can be used as a starting point for developing Laravel apps with Docker.

You can check this medium [post](https://medium.com/@mrfoh/developing-laravel-applications-with-docker-7324c0a0789a) out for more information.

This setup contains;

 - PHP-FPM (PHP 7)
 - Nginx web server
 - MySQL database

## Run
Make sure your have composer and [Docker](https://docs.docker.com/) installed

Clone the repo

    git clone https://github.com/mrfoh/docker-laravel.git

 Change directory

    cd docker-laravel
  Install dependencies

    composer install
  Build and run the Docker containers

    docker-compose up -d
   This builds the containers and runs them in the background, while this


    docker-compose up
   builds the containers to outputs their logs to the console.
   You should be able to visit your app at http://localhost:8080

To stop the containers run `docker-compose kill`, and to remove them run `docker-compose rm`
