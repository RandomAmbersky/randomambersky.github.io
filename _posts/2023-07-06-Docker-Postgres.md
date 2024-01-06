---
layout: post
title: Подключение к внешней БД Postgres из Docker
---

Качаем Postgres.app для MacOs тут - https://postgresapp.com

Комментарим весь сервис `postgres` в `docker-compose.yml`

Меняем параметр коннекта в `connection.env` :

```bash
DATABASE_CONNECTION_URI=postgres://postgres@host.docker.internal/maskeddata
```
