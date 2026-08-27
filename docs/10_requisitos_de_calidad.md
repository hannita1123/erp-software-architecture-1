# Requisitos de Calidad

## Árbol de calidad

A continuación se listan los atributos de calidad más importantes para
el Sistema ERP, con un escenario concreto que los ilustra:

### Usabilidad
- **Escenario:** el Administrador de Compras debe poder registrar un
  nuevo producto en menos de 1 minuto, gracias a un formulario simple
  y claro en la SPA.

### Rendimiento
- **Escenario:** al consultar el historial de órdenes de compra, la
  API debe responder en menos de 2 segundos, incluso con miles de
  registros almacenados.

### Confiabilidad
- **Escenario:** si la conexión entre la SPA y la API falla, la SPA
  debe mostrar un mensaje de error claro al usuario, sin perder los
  datos que ya había ingresado en el formulario.

### Mantenibilidad
- **Escenario:** un nuevo desarrollador debe poder entender la
  estructura del proyecto (SPA, API, BD) y realizar un cambio simple
  (como agregar un campo a un formulario) en menos de un día,
  gracias a la separación clara de responsabilidades entre capas.

### Seguridad
- **Escenario:** toda la información sensible (como datos de
  proveedores) debe viajar cifrada mediante HTTPS entre la SPA y
  la API, evitando que terceros intercepten los datos.
