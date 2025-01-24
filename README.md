# Comandos dockert

## Revisar docker ejecutados
Ejeutar: docker ps

## Revisar imagenes de docker
Ejecutamos: docker images

## Crear docker
Ejecutar: docker build .
Ejecutar: docker build -t nombrerepositorio:tag .

## Eliminar la imagen
Ejecutar: docker rmi <ID imagen>

## Forsar eleiminar imagen
Ejecutar: docker rmi -f <ID imagen>


## Ejecutar la imagen
docker run -it --rm -d -p 8080:80 --name web sitioweb
docker run -it --rm -d -p 8080:80 --name web -v ${PWD}/sitio:/usr/share/nginx/html web:sitioweb
