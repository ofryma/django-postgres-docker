this repo follows [this tutorial](https://testdriven.io/blog/dockerizing-django-with-postgres-gunicorn-and-nginx/).


create `.env` file in the root directory.
```
DEBUG=1
SECRET_KEY=foo
DJANGO_ALLOWED_HOSTS=localhost 127.0.0.1 [::1]
SQL_ENGINE=django.db.backends.postgresql
SQL_DATABASE=db_name_here
SQL_USER=db_user_here
SQL_PASSWORD=db_password_here
SQL_HOST=db
SQL_PORT=5432
DATABASE=postgres
```

```
docker-compose --env-file .env up -d --build
```

