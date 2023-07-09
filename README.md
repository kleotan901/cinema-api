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
set POSTGRES_HOST=<your db hostname>
set POSTGRES_DB=<your db name>
set POSTGRES_USER=<your db username>
set POSTGRES_PASSWORD=<your db password>
python manage.py migrate
python manage.py runserver
```


## Run with docker

Docker should be installed

```shell
docker-compose build
docker-compose run
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
