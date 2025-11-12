# MS Pedidos

Microservicio de pedidos.

## Dependencias
- PostgreSQL con DB db_pedidos_dev/qa/prd.
- Ejecutar `database/script.sql`.
- ms-productos corriendo.

## Ejecutar
- `./gradlew bootRun` (dev: 8082, qa: 8084, prd: 8086).
- Perfil: `--spring.profiles.active=dev`.

## Endpoints
- GET /api/pedidos
- GET /api/pedidos/{id}
- POST /api/pedidos
- PUT /api/pedidos/{id}/estado
- DELETE /api/pedidos/{id}

## Ejemplo POST pedido
```json
{
  "cliente": "Juan",
  "detalles": [
    {"productoId": 1, "cantidad": 2}
  ]
}
