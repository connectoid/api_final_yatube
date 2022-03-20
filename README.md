### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/api_final_yatube.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```

Примеры запросов к API:

```
GET   /api/v1/posts/                          - получить список всех публикаций
POST  /api/v1/posts/                          - создание новой публикации
GET   /api/v1/posts/{id}/                     - получить публикацию по id
POST  /api/v1/posts/{post_id}/comments/       - добавление коментария к публикации
GET   /api/v1/posts/{post_id}/comments/{id}/  - получение комментария к публикации по id
```
