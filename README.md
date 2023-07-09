# Cinema-API

API service for cinema management written on DRF

## Installing using GitHub

Install PostgresSQL and create db

```shell
git clone https://github.com/kleotan901/cinema-api.git
cd cinema-api
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

## Configuration
The project uses environment variables for configuration. Please follow these steps to set up the required configuration files.

###  .env and .env.sample file
The .env file is used to store sensitive information and configuration variables that are necessary for the project to function properly.

The .env.sample file serves as a template or example for the .env file. It includes the necessary variables and their expected format, but with placeholder values.

To configure the project:

Locate the .env.sample file in the project's root directory.
Duplicate the .env.sample file and rename the duplicated file to .env.
Open the .env file and replace the placeholder values with the actual configuration values specific to your setup.
Remember to keep the .env file secure and avoid sharing it publicly or committing it to version control systems.


## Run with docker

Docker should be installed

* Use .dockerignore for ignoring unnecessary stuff in your images;
* Use Dockerfile for building app image with DRF application;
* Use docker-compose.yml file for managing multiple services (containers) at the same time;

```shell
docker-compose build
docker-compose up
```
## Getting access
* Create user via api/user/register
* Get access token via api/user/token

## Features

* JWT Authenticated
* Admin panel /admin/
* Documentation is located at api/doc/swagger/
* Managing orders and tickets
* Creating movies with genres, actors
* Creating cinema hall
* Adding movie sessions
* Filtering movies and movies sessions
