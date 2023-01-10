# docker-compose commands
build:
```shell
docker-compose build
```
flake8 linting(only in DEV):
```shell
docker-compose run --rm app sh -c "flake8"
```
run test:
```shell
docker-compose run --rm app sh -c "python manage.py test"
```
create django project:
```shell
docker-compose run --rm app sh -c "django-admin startproject app ."
```
run project:
```shell
docker-compose up
```