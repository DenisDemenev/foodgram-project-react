![example workflow](https://github.com/DenisDemenev/foodgram-project-react/actions/workflows/foodgram_workflow.yml/badge.svg)  

### Описание проекта:

Проект собирает рецепты блюд от пользователей , позволят подписываться на интересных авторов, добавлять рецепты в избраное и помогает сформировать корзину для покупок ингредиентов для выбранных рецептов.

Проект доступен по адресу: http://51.250.12.61/

#### Технологии
Django, DRF, PostreSQL, React(Яндекс.Практикум)


#### Установка:

Установите docker и docker-compose Инструкция по установке доступна в официальной документации

#### Создайте файл .env с переменными окружения:

DB_ENGINE=django.db.backends.postgresql</br>
DB_NAME=<ваши_данные> # Имя базы данных</br>
POSTGRES_USER=<ваши_данные> # Администратор базы данных</br>
POSTGRES_PASSWORD=<ваши_данные> # Пароль администратора</br>
DB_HOST=<ваши_данные></br>
DB_PORT=5432</br>

#### Собрать и запустить контейнер:

docker-compose up -d --build

#### Миграции:

sudo docker-compose exec -T backend python manage.py makemigrations --noinput</br>
sudo docker-compose exec -T backend python manage.py migrate --noinput

#### Создайте суперпользователя:

sudo docker-compose exec backend python manage.py createsuperuser


Автор: Денис Деменев