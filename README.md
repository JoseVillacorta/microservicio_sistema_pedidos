# Sistema de Gestión de Pedidos

## Instalación
- Instalar Java 21, PostgreSQL, Git.
- Clonar repo.

## Configuración DB
- Crear DBs: db_productos_dev/qa/prd, db_pedidos_dev/qa/prd.
- Ejecutar scripts en database/.

## Ejecutar
- ms-config-server: `./gradlew bootRun` (puerto 8888).
- ms-productos: `./gradlew bootRun` (dev: 8081).
- ms-pedidos: `./gradlew bootRun` (dev: 8082).

## Endpoints
- Productos: GET/POST/PUT/DELETE /api/productos, GET /api/productos/bajo-stock.
- Pedidos: GET/POST/PUT/DELETE /api/pedidos, PUT /api/pedidos/{id}/estado.

## Ejemplos
- Crear producto: POST /api/productos con JSON {nombre, precio, stock}.
- Crear pedido: POST /api/pedidos con JSON {cliente, detalles: [{productoId, cantidad}]}.
