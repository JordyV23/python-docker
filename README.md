# Comandos útiles de Docker

A continuación se muestran algunos comandos útiles de Docker para gestionar imágenes y contenedores.

## Gestionar imágenes

### Lista de imágenes

$ docker image ls

### Eliminar una imagen específica

$ docker image rm [nombre de la imagen]

### Eliminar todas las imágenes existentes

$ docker image rm $(docker images -a -q)

## Gestionar contenedores

### Lista de todos los contenedores existentes (en funcionamiento y no en funcionamiento)

$ docker ps -a

### Detener un contenedor específico

$ docker stop [nombre del contenedor]

### Detener todos los contenedores en funcionamiento

$ docker stop $(docker ps -a -q)

### Eliminar un contenedor específico (solo si está detenido)

$ docker rm [nombre del contenedor]

### Eliminar todos los contenedores (solo si están detenidos)

$ docker rm $(docker ps -a -q)

## Mostrar los registros de un contenedor

$ docker logs [nombre del contenedor]
