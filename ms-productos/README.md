# MS Productos

Microservicio de productos reactivo.

## Dependencias
- PostgreSQL con DB db_productos_dev/qa/prd.
- Ejecutar `database/script.sql`.

## Ejecutar
- `./gradlew bootRun` (dev: 8081, qa: 8083, prd: 8085).
- Perfil: `--spring.profiles.active=dev`.

## Endpoints
- GET /api/products
- GET /api/products/{id}
- POST /api/products
- PUT /api/products/{id}
- PUT /api/products/{id}/stock
- DELETE /api/products/{id}
- GET /api/products/bajo-stock

## Ejemplo POST producto
```json
{
  "nombre": "Producto",
  "descripcion": "Desc",
  "precio": 100.0,
  "stock": 10
}
