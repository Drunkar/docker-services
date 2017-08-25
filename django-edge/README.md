# django-edge

django with edge template http://django-edge.readthedocs.io/en/latest/ and postgresql.


## Usage

### 1. Change db name and password

- `POSTGRES_USER`: user and db name
- `POSTGRES_PASSWORD`: password for `POSTGRES_USER`

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
