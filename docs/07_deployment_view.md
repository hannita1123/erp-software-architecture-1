# Vista de Despliegue

## Descripción
Esta sección describe, de forma general, cómo se desplegaría la
arquitectura del Sistema ERP en un entorno de producción.

## Infraestructura propuesta
- La **Single-Page Application (SPA)** se despliega como archivos
  estáticos (HTML, CSS, JS) servidos a través de un servidor web o un
  servicio de hosting como Nginx.
- La **API Monolítica** (Java, Spring Boot) se despliega en un servidor
  de aplicaciones o contenedor (por ejemplo, Docker), expuesto mediante
  HTTPS.
- La **Base de Datos PostgreSQL** se despliega en un servidor dedicado
  o en un servicio administrado de base de datos en la nube.

## Comunicación
- El navegador del usuario se conecta a la SPA mediante HTTPS.
- La SPA se comunica con la API mediante peticiones HTTPS/JSON.
- La API se comunica con la base de datos mediante el protocolo JDBC,
  dentro de una red privada para mayor seguridad.
