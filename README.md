
# Yatube API

Простой API для нашей платформы мини-блогов Yatube.
***
### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```bash
git clone https://github.com/KapkaDibab/api_final_yatube.git
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
## Примеры работы с API

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




## Авторы

- [@yandex-praktikum](https://github.com/yandex-praktikum)
- [@KapkaDibab](https://github.com/KapkaDibab)


