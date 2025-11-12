# Config Repo

Repositorio Git para configuraciones centralizadas.

## Estructura
- `ms-productos-dev.yml`: Config dev para ms-productos (DB db_productos_dev, puerto 8081).
- `ms-productos-qa.yml`: Config QA (DB db_productos_qa, puerto 8083).
- `ms-productos-prd.yml`: Config PRD (DB db_productos_prd, puerto 8085).
- `ms-pedidos-dev.yml`: Config dev para ms-pedidos (DB db_pedidos_dev, puerto 8082).
- `ms-pedidos-qa.yml`: Config QA (DB db_pedidos_qa, puerto 8084).
- `ms-pedidos-prd.yml`: Config PRD (DB db_pedidos_prd, puerto 8086).
- `registry-service.yaml`: Config para registry-service (puerto 8761).
- `gateway-service.yaml`: Config para gateway (puerto 8080).

## Uso
- Commitea cambios: `git add . && git commit -m "Update"`.
- MS cargan configs via Config Server en `http://localhost:8888`.
