# QRKot - приложение для Благотворительного фонда с возможностью формирования отчёта в гугл-таблице

## Возможности проекта QRKot

- Создание благотворительных проектов
- Внесение пожертвований пользователями
- Автоматическое поступление пожертвований в открытые проекты
- Регистрация пользователей на основе FastAPI Users
- New! Добавлена возможность формирования отчёта в гугл-таблице

## Технологии

<p align="left"> 
<a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"> </a>
<a href="https://www.sqlalchemy.org/" target="_blank" rel="noreferrer"> <img src="https://github.com/devicons/devicon/blob/master/icons/sqlalchemy/sqlalchemy-original.svg" alt="sqlalchemy" width="40" height="40"> </a>
<a href="https://fastapi.tiangolo.com/" target="_blank" rel="noreferrer"><img src="https://github.com/devicons/devicon/blob/master/icons/fastapi/fastapi-original.svg" alt="fastapi" width="40" height="40"> </a>
<a href="https://github.com/sqlalchemy/alembic" target="_blank" rel="noreferrer"><img src="https://github.com/awkward/Alembic/blob/master/Docs/icon.png" alt="alembic" width="40" height="40"> </a>
<a href="https://github.com/fastapi-users/fastapi-users" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/fastapi-users/fastapi-users/master/logo.svg" alt="fastapi-users" width="120" height="40"> </a>
</p>

## Установка и запуск проекта

- В корневой папке создайте файл *.env* и добавьте в него свои данные (при необходимости):

```
APP_TITLE=Приложение QRKot
APP_DESCRIPTION=Приложение для благотворительного фонда.
DATABASE_URL=sqlite+aiosqlite:///./fastapi.db
SECRET=secret
FIRST_SUPERUSER_EMAIL=admin@admin.com
FIRST_SUPERUSER_PASSWORD=admin
TYPE=service_account
PROJECT_ID=your_projectid
PRIVATE_KEY_ID=your_private_key
PRIVATE_KEY=-----BEGIN PRIVATE KEY-----your_private_key-----END PRIVATE KEY-----
CLIENT_EMAIL=client@your_projectid.iam.gserviceaccount.com
CLIENT_ID=123456789012345678901
AUTH_URI=https://accounts.google.com/o/oauth2/auth
TOKEN_URI=https://oauth2.googleapis.com/token
AUTH_PROVIDER_X509_CERT_URL=https://www.googleapis.com/oauth2/v1/certs
CLIENT_X509_CERT_URL=https://www.googleapis.com/robot/v1/metadata/x509/client%40your_projectid=.iam.gserviceaccount.com
EMAIL=your@gmail.com
```
- Установите зависимости

- Создайте миграции

```shell
alembic revision --autogenerate -m "First migration" 
```

- Установите миграции

```shell
alembic upgrade head
```

- Запустите проект

```shell
uvicorn main:app  --reload
```

## Документация проекта

После запуска проекта откройте одну из ссылкок в браузере:

```shell
http://127.0.0.1:8000/docs
```

```shell
http://127.0.0.1:8000/redoc
```

## Над проектом работали:

- [Денисова Яна](https://t.me/DenisovaYana)
