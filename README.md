#Django-environments

## Para crear el proyecto en Django:
docker-compose run web django-admin.py startproject django_environments webapp/  

## Para levantar el docker:
docker-compose up -d

## Para bajar el docker:
docker-compose down

## Para ver los logs de la base de datos:
docker-compose log db.

## Para ver los logs del proyecto:
docker-compose log webapp

###Buenas Prácticas

Las variables del entorno estan definidas en el .env (noten el . precedente en el archivo para hacerlo oculto).
Este archivo NO deben incluirlo es su repositorio por obvias razones.
