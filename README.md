
# Yatube API

Простой API для нашей платформы мини-блогов Yatube.


### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```bash
git clone https://github.com/Esedess/api_final_yatube.git
```

```bash
cd yatube_api
```

Cоздать и активировать виртуальное окружение:

```bash
python -m venv env
```

```bash
source env/bin/activate
```

Установить зависимости из файла requirements.txt:

```bash
python -m pip install --upgrade pip
```

```bash
pip install -r requirements.txt
```

Выполнить миграции:

```bash
python manage.py migrate
```

Запустить проект:

```bash
python manage.py runserver
```


## API Reference

#### Получить все посты

```http
  GET api/v1/posts/
```

| Headers | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Authorization` | `string` | **Required**. Bearer <JWT-Token> |

#### Сделать пост

```http
  POST api/v1/posts/
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `text`      | `string` | **Required**. Текст поста |




## Tech Stack

[Django](https://github.com/django/django)

[Django REST framework](https://github.com/encode/django-rest-framework)

[djoser](https://github.com/sunscrapers/djoser)



## Авторы

- [@yandex-praktikum](https://github.com/yandex-praktikum)
- [@Esedess](https://github.com/Esedess)


