Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:

git clone https://github.com/Fedoska48/api_final_yatube.git
cd yatube_api
Cоздать и активировать виртуальное окружение:

python -m venv env
source venv/Source/activate
Установить зависимости из файла requirements.txt:

python -m pip install --upgrade pip
pip install -r requirements.txt
Выполнить миграции:

python manage.py migrate
Запустить проект:

python3 manage.py runserver