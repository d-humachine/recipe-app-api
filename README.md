# startup commands
#### build:
```shell
docker-compose build
```

#### run project:
```shell
docker-compose up
```

# commands reference
#### flake8 linting(only in DEV):
```shell
docker-compose run --rm app sh -c "flake8"
```

#### run test:
```shell
docker-compose run --rm app sh -c "python manage.py test"
```

#### create django project:
```shell
docker-compose run --rm app sh -c "django-admin startproject app ."
```

#### add django core app (with wait_for_db func):
```shell
docker-compose run --rm app sh -c "python manage.py startapp core"
```

#### check custom django command wait_for_db
```shell
docker-compose run --rm app sh -c "python manage.py wait_for_db"
```