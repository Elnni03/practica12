# Práctica 12 — Monitoreo con Prometheus y Grafana

Práctica para configurar monitoreo usando Prometheus y Grafana con Docker Compose.

## Requisitos
- Docker instalado
- Docker Compose instalado

## Levantar el sistema
```bash
docker-compose up -d
```

## Servicios
| Servicio      | URL                   |
|---------------|-----------------------|
| Prometheus    | http://localhost:9090 |
| Grafana       | http://localhost:3000 |
| Node Exporter | http://localhost:9100 |

## Configurar Grafana
1. Entra a http://localhost:3000 (usuario: admin / contraseña: admin)
2. Ve a Configuration > Data Sources > Prometheus
3. URL: http://prometheus:9090 → Save & Test

## Detener
```bash
docker-compose down
```
