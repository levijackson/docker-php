# Docker PHP
Simple container setup to test standalone PHP code without a web server. Mainly just proof of concept and unit-testable code.

# Setup
Copy `.env.example` => `.env` and set the path to the PHP code you want to run.

# Usage
1) `docker-compose run composer install` - installs all the composer dependencies
2) `docker-compose run php vendor/bin/phpunit` - executes unit tests