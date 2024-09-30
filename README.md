## Client Gateway
El gateway es el punto de comunicación entre nuestros clientes y nuestros servicios.
Es el encargado de recibir las preticiones, enviarlas a los servicios correspondientes y devolver la respuesta al cliente.

## Dev
1. Clonar le repositorio
2. Instalar dependencias
3. Crear un archivo `.env` basado en el `.env.example`
4. Levantar el servidor de nats
```
docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
```
5. Tener levantados los microservicios que se van a consumir
6. Levantar proyecto con `npm run start:dev`

## Nats
```
docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
```