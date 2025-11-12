# Sistema de Microservicios: Gestión de Pedidos

Arquitectura completa con Spring Boot, WebFlux, R2DBC, PostgreSQL, Config Server, Eureka, Gateway.

## Instalación
- Instalar Java 21, PostgreSQL, Git.
- Clonar repo.

## Servicios
- **ms-config-server**: Config Server (puerto 8888)
- **registry-service**: Eureka Server (puerto 8761)
- **gateway**: API Gateway (puerto 8080)
- **ms-productos**: Productos reactivos (puerto 8081)
- **ms-pedidos**: Pedidos reactivos (puerto 8082)

## Inicio Rápido
1. Crear DBs en PostgreSQL: db_productos_dev, db_pedidos_dev.
2. Ejecutar scripts en database/.
3. `./gradlew bootRun` en cada servicio (orden: config-server, registry, gateway, ms-productos, ms-pedidos).
4. Acceder via Gateway: `http://localhost:8080/api/products`

## Documentación
Ver README en cada carpeta.
