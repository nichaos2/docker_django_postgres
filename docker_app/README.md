# Docker django postgresql


Tutorial
--------

Follow instruction from [a link](https://testdriven.io/blog/dockerizing-django-with-postgres-gunicorn-and-nginx/)

* Note: to create requirements file give the command

```shell
pip freeze > requirements.txt
```


Prerequisites
-------------

You need to have installed: Docker, Postgresql and Python 3.


Uses the following stack
------------------------

* Docker
    - Develoment and 
    - Production
* Postgresql
    - with the library psycopg2-binary
* GUnicorn
    - As Server
* Nginx
    - As Reverse Proxy


Launch
------

Development: 

```shell
docker-compose -f docker-compose.yml up -d --build
```

Then got to page localhost:8000

Production

```shell
docker-compose -f docker-compose.prod.yml up -d --build
```

Remember to take down the image before with docker-compose -f docker-compose.yml or docker-compose.prod.yml down -v