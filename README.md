# Описание:
Проект API для YATUBE.
Реализвоана возможность взаимодействие с проэктом через API.


Возможности:

1. Созднание,редактирование, удаление и просмотр записей, коментариев к записям, для неаутентифицированных пользватель доступен только просмотр.
2. Оформлени подписки\ отписки на авторов только для аутентифицированных  пользователей.
3. Для аутентификации используется JWT-токенс ограниченым временем действия.


# Установка:

1. Сделать форк репозмториию в свой профиль.
2. Клонировать репозиторий на свое устройство в нужную дерикторию.
3. Установить virtualvenv "python -m venv venv" и активировать его "source venv/Scripts/activate"
4. Установите зависимости "pip install -r requirements.txt"
5. После перейти в дерикторию c коммандной утилитой manage.py и приминить миграции "python manage.py migrate"
6. Запустите проэкт "python manage.py runserver"

# Примеры:
1. /api/v1/jwt/create/ - получения JWT-токен (POST)
2. /api/v1/posts/ - список всех постов (POST, GET)
3. /api/v1/posts/{post_id}/ - подробная информации о посте (POST, GET, PUT, PATCH, DELETE)
4. /api/v1/follow/ - список подписок на аторов