<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

## Client Gateway
El gateway  es el punto de entrada para las solicitudes realizadas por los clientes recibirlas y comunicarlas a nuestros microservicios asi como recibir una respuesta de nuestros microservicios y devolverla al cliente.


## Dev

1. Clonar el repositorio.
2. Instalar las dependencias `npm install`.
3. Crear un archivo `.env` basado en el archivo `.env.template`
4. Levantar el servidor de NATS
```
docker run -d --name nats-main -p 4222:4222 -p 6222:6222 -p 8222:8222 nats
```
5. Tener levantados los microservicios que se van a consumir.
6. Levantar la aplicacion `npm run start:dev`.


## Nats
```
docker run -d --name nats-main -p 4222:4222 -p 6222:6222 -p 8222:8222 nats
```