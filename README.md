# Theatre API

API service for theatre management written on DRF

## Installing using GitHub:

Install PostgresSQL and create db

'''shell
- git clone https://github.com/IvanGuculyak/Theatre-API-Service.git
- cd theatre_API
- python3 -m venv venv
- source venv/bin/activate
- pip install -r requirements.txt
- set DB_HOST=<your db hostname>
- set DB_NAME=<your db name>
- set DB_USER=<your db username>
- set DB_PASSWORD=<your db user password>
- set SECRET_KEY=<your secret key>
- python manage.py migrate
- python manage.py runserver  # starts Django Sever
'''

## Run with docker

Docker should be installed

'''shell
- docker-compose build
- docker-compose up
'''

## Gettings access

'''shell
- create user via /api/user/register/
- get access token via /api/user/token/
'''

## Features

- JWT authenticated
- Admin panel /admin
- Documentation is located at /api/doc/swagger/
- Managing reservations and tickets
- Creating plays with genres, actors
- Creating theatre halls
- Adding performances
- Filtering plays and performances

## Scheme of DB:

![scheme_of_db.jpg](scheme_of_db.jpg)
