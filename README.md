# Vue-Django
Django project with an integration of vuejs 

### Features

* Django backend in `./backend`
* vuejs frontend in `./frontend`
* Hot-reload with vue-loader
* eslint linter integration
* Makefile to make your life easy


### Development environment setup

```bash
make dev
make migrate
make run
```

or 

```bash
Run Django 
python3 manage.py runserver 8000
```
```bash
Run Npm
npm run dev
```

### Deployment

```bash
make prod
make build
```

