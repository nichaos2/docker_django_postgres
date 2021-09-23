# Docker django postgresql

* Tutorial

Follow instruction from [a link](https://testdriven.io/blog/dockerizing-django-with-postgres-gunicorn-and-nginx/)

* Prerequisites

You need to have installed: Docker, Postgresql and Python 3.

* Note: to create requirements file give the command

```shell
pip freeze > requirements.txt
```

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