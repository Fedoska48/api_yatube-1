## Приложение позволяет взаимодействовать с yatube по API
**Технологический стек:**
- Python 3<br/>

- Django<br/>
- Django REST Framework

***
### Как запустить проект:

**Клонировать репозиторий и перейти в него в командной строке:**<br/>
git clone https://github.com/Fedoska48/api_final_yatube.git <br/>
cd yatube_api

**Cоздать и активировать виртуальное окружение:**<br/>
python -m venv env <br/>
source venv/Source/activate

**Установить зависимости из файла requirements.txt:**<br/>
python -m pip install --upgrade pip <br/>
pip install -r requirements.txt

**Выполнить миграции:**<br/>
python manage.py migrate

**Запустить проект:**<br/>
python manage.py runserver
***

## Возможности
**Аутентифицировнный пользователь или только чтение**

Модель Post: операций CRUD (создание для аутентифицировнных юзеров, апдейт и делит для авторов) <br/>

Модель Comment: операций CRUD (создание для аутентифицировнных юзеров, апдейт и делит для авторов) <br/>

Модель Group: ReadOnly для всех <br/>

**Только для аутентифицированных пользователей**

Модель Follow: получить список пользователей на кого подписан пользователь, добавить новую подписку

***

## Работа с токенами релизована на основе JWT + Djoser:
Эндпойты Djoser: /auth/ <br/>
Эндпойты JWT: /api/v1/

***
### Redoc
Описание API доступно по адресу **/redoc/**
