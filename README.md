# Docker PHP
Simple container setup to test standalone PHP code without a web server. Mainly just proof of concept and unit-testable code.


# Usage
1a) Copy `.env.example` => `.env` and set the path to the PHP code you want to run.

1b) use an inline environment variable to set the application path `APPLICATION_PATH=/path/to/code/ docker-compose run ...`

2) `docker-compose run composer install` - installs all the composer dependencies

3) `docker-compose run php vendor/bin/phpunit` - executes unit tests