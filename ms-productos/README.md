# MS Productos

Microservicio de productos.

## Dependencias
- PostgreSQL con DB db_productos_dev/qa/prd.
- Ejecutar `database/script.sql`.

## Ejecutar
- `./gradlew bootRun` (dev: 8081, qa: 8083, prd: 8085).
- Perfil: `--spring.profiles.active=dev`.

## Endpoints
- GET /api/productos
- GET /api/productos/{id}
- POST /api/productos
- PUT /api/productos/{id}
- PUT /api/productos/{id}/stock
- DELETE /api/productos/{id}
- GET /api/productos/bajo-stock

## Ejemplo POST producto
```json
{
  "nombre": "Producto",
  "descripcion": "Desc",
  "precio": 100.0,
  "stock": 10
}
