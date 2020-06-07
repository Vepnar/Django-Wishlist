# Django-Wishlist
This is a sample project

## WORK IN PROGRESS

## Installation
1. First you need to clone our repository
`git clone https://github.com/Vepnar/Django-Wishlist.git`

3. add .env files to the required directectoires `/app` & `/db`

2. After that you need to run docker
`docker-compose build && docker-compose up`

3. Collect all static files `docker-compose exec app python manage.py migrate --no-input`

4. Now you need to initialize the PostgreSQL database
`docker-compose exec app python manage.py migrate --no-input`


