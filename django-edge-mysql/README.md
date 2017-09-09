# django-edge-mysql

django with edge template http://django-edge.readthedocs.io/en/latest/ and mysql.
mysql store twitter-streaming-api data.


## Usage

### 1. Set db name and password

in `db-variables.env` file

- `MYSQL_ROOT_PASSWORD`, `DB_ENV_MYSQL_ROOT_PASSWORD`: must be the same. db root user password.

### 2. Up

```
docker-compose up -d
```

### 3. Create a superuser

```
docker exec -it djangoedgemysql_web_1 bash

# in the container
cd my_proj/src/ && python manage.py createsuperuser
exit
```
