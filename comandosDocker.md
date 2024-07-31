## Para Instalar nats, no publicamos el puerto -p 6222:6222 y se inatalara la latest por defecto
```
docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
```

## Para construir una imagen
```
docker compose up -d --build
```

## Para Instalar nats en cada microservicio incluido el client-gateway
```
npm i --save nats
```
## Para crear un modulo personalizado que sera utilizado en todos los modolos de gateway-ms (clientes,cuentas,movimientos y reportes)
```
nest g mo nats
```