# yamdb_final
yamdb_final

## Что это за проект?

```
> Это API для проекта Yamdb, позволяющая получать, удалять, редактировать
> данные о произведениях и пользователях, оставлять комментарии и отзывы к произведениям
> Произведения удобно распределены по категориям и жанрам
> Все данные возвращаются в формате JSON
```

## Как запустить проект:

### 1.
```
Установить программу Docker и плагин docker compose
```

### 2.
```
Клонировать репозиторий
git clone git@github.com:Serenityblood/yamdb_final.git
```

### 3.
```
Для корректной работы проекта потребутеся создать и заполнить файл .env
cd yamdb_final/infra
touch .env
DB_ENGINE=django.db.backends.postgresql
DB_NAME=postgres
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
DB_HOST=db
DB_PORT=5432
```

### 3.
```
docker-compose up -d
```

### 4.
```
Сделать миграции 
docker-compose exec web python manage.py makemigrations
```

## Исопользуемые технологии
```
requests==2.26.0
django==2.2.16
djangorestframework==3.12.4
PyJWT==2.1.0
pytest==6.2.4
pytest-django==4.4.0
pytest-pythonpath==0.7.3
djangorestframework-simplejwt==4.8.0
django-filter==21.1
```


## Авторы проекта:
```
> Serenity(Users/Auth), Lolozius(Serializers/Views), Nail(Models)
```

## IP проекта:
```
http://158.160.24.255/
```

## Документация:
```
http://158.160.24.255/redoc
```
[![Django-app workflow](https://github.com/Serenityblood/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)](https://github.com/Serenityblood/yamdb_final/actions/workflows/yamdb_workflow.yml)