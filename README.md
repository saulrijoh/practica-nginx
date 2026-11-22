# Práctica de Nginx con Docker Compose

Servidor web local que muestra «Hola mundo» usando Nginx y Docker Compose.

## Ejecución con Colima

Inicia Colima si todavía no está en ejecución y selecciona su contexto:

```bash
colima start
docker context use colima
docker compose up -d
```

Abre <http://localhost:8080>. La carpeta `src` se monta en el directorio de contenido de Nginx; los cambios en `src/index.html` se reflejan al actualizar la página.

Para detener el contenedor:

```bash
docker compose down
```

Si tu instalación dispone del comando independiente `docker-compose`, puedes usarlo en lugar de `docker compose`.
