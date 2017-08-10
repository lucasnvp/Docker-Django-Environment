# Django-environments

## Para crear el proyecto en Django:
`docker-compose run web django-admin.py startproject django_environments webapp/`

## Para construir el proyecto:
`docker-compose build`

## Para levantar el docker:
`docker-compose up -d`

## Para bajar el docker:
`docker-compose down`

## Para crear una aplicación dentro del proyecto Django se utiliza el siguiente comando:
`docker-compose run web python manage.py startapp app`

## Los usuarios se crean utilizando el mismo comando descrito en la documentación de Django.
`docker-compose run web python manage.py createsuperuser`

## Para migrar las clases a la base de datos
`docker-compose run web python manage.py migrate`

## Para borrar una tabla de la base de datos
name_app se reemplaza por el nombre de la aplicacion. 
`docker-compose run web rm -r name_app/migrations`

## Para ver los logs de la base de datos:
`docker-compose logs db`

## Para ver los logs del proyecto:
`docker-compose logs webapp`

### Buenas Prácticas

Las variables del entorno estan definidas en el .env (noten el . precedente en el archivo para hacerlo oculto).
Este archivo NO deben incluirlo es su repositorio por obvias razones.
