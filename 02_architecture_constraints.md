# Restricciones de Arquitectura

## Decisiones tecnológicas

- **Backend:** Java con Spring Boot, expuesto como una API REST monolítica
  que centraliza toda la lógica de negocio.
- **Base de datos:** PostgreSQL, como motor relacional para almacenar
  productos, proveedores, órdenes de compra y demás entidades del ERP.
- **Frontend:** Aplicación de una sola página (SPA) construida con
  JavaScript/React, que consume la API mediante peticiones HTTPS/JSON.
- **Comunicación:** Toda la comunicación entre la SPA y la API se realiza
  mediante HTTPS, y entre la API y la base de datos mediante JDBC.

## Restricciones organizativas
- El equipo de desarrollo cuenta con experiencia previa en el ecosistema
  Java/Spring, lo que motiva la elección del backend.
- Se prioriza una arquitectura simple (monolito) dado el tamaño inicial
  del proyecto, dejando abierta la posibilidad de evolucionar a
  microservicios en el futuro.
