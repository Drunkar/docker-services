# django-edge

django with edge template http://django-edge.readthedocs.io/en/latest/ and postgresql.


## Usage

### 1. Set db name and password

in `db-variables.env` file

- `POSTGRES_USER`, `DB_ENV_POSTGRES_USER`: must be the same. user name.
- `POSTGRES_PASSWORD`, `DB_ENV_POSTGRES_PASSWORD`: must be the same. user password.

### 2. Up

```
docker-compose up -d
```

### 3. Create a superuser

```
docker exec -it djangoedge_web_1 bash

# in the container
cd my_proj/src/ && python manage.py createsuperuser
exit
```
