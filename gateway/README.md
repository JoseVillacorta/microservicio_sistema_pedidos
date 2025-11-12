# Gateway

API Gateway usando Spring Cloud Gateway.

## Ejecutar
- `./gradlew bootRun` (puerto 8080).
- Verifica Eureka: `http://localhost:8761` (debe aparecer gateway-service).

## Rutas
- `/api/products/**` -> lb://ms-productos
- `/api/pedidos/**` -> lb://ms-pedidos

## Configuración
- Config Server: http://localhost:8888
- Eureka: http://localhost:8761