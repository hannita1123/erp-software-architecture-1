# Vista de Bloques de Construcción

## Descripción general
Esta sección detalla los principales "contenedores" (bloques técnicos)
que componen el Sistema ERP, mostrando de qué piezas está hecho y cómo
se relacionan entre sí.

A continuación se muestra el diagrama de contenedores (C2) del sistema:

![Diagrama de Contenedores](c2_contenedores.png)

## Responsabilidad de cada contenedor

### Single-Page Application (SPA)
- **Tecnología:** JavaScript, React.
- **Responsabilidad:** es la interfaz de usuario que se ejecuta en el
  navegador. Permite al Administrador de Compras registrar productos,
  proveedores y órdenes de compra, comunicándose con la API mediante
  peticiones HTTPS/JSON.

### API Monolítica
- **Tecnología:** Java, Spring Boot.
- **Responsabilidad:** concentra toda la lógica de negocio del ERP:
  validación de datos, reglas de negocio de compras, cálculo de totales
  de órdenes, y comunicación con la base de datos.

### Base de Datos
- **Tecnología:** PostgreSQL.
- **Responsabilidad:** almacena de forma persistente todos los datos del
  ERP (productos, proveedores, órdenes de compra, stock, etc.), a los
  que la API accede mediante JDBC.
