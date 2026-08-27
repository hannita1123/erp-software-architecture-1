# Conceptos Transversales

## Manejo de errores
Todas las peticiones a la API que fallen (por ejemplo, datos inválidos
o recursos no encontrados) devuelven un código de error HTTP adecuado
(400, 404, 500) junto con un mensaje descriptivo, que la SPA muestra
al usuario de forma clara.

## Validación de datos
La validación de los datos ingresados por el usuario se realiza en dos
niveles:
- **Frontend (SPA):** validaciones básicas antes de enviar la petición
  (campos obligatorios, formatos).
- **Backend (API):** validaciones de negocio más estrictas, que son la
  fuente de verdad final antes de guardar en la base de datos.

## Seguridad
- Toda la comunicación entre la SPA, la API y los sistemas externos se
  realiza mediante HTTPS.
- Se contempla la implementación de autenticación y autorización para
  que solo usuarios autorizados puedan registrar productos, proveedores
  y órdenes de compra.

## Persistencia de datos
Todas las entidades del Módulo de Compras (Producto, Proveedor, Orden
de Compra) se almacenan en la base de datos PostgreSQL, siguiendo el
modelo relacional definido en el Diagrama de Entidad-Relación (MER).
