# Estrategia de Solución

## Decisiones clave de arquitectura
- Se optó por una **arquitectura monolítica** en lugar de microservicios,
  dado el tamaño inicial del proyecto y el equipo de desarrollo disponible.
- Se eligió **Spring Boot** por ser un framework maduro, con amplia
  documentación y soporte para construir APIs REST de forma rápida y segura.
- Se eligió **PostgreSQL** como base de datos relacional por su robustez,
  soporte de transacciones ACID y buena integración con Java.
- El frontend se construye como una **SPA en React**, lo que permite una
  experiencia de usuario fluida sin recargar la página completa.

## Cómo se abordan los objetivos de calidad
- **Mantenibilidad:** al separar claramente frontend (SPA), backend (API)
  y base de datos, cada capa puede evolucionar de forma independiente.
- **Escalabilidad futura:** aunque hoy es un monolito, la separación clara
  de responsabilidades facilita una futura migración a microservicios.
- **Seguridad:** toda la comunicación se realiza mediante HTTPS, y la
  validación de datos se hace tanto en el frontend como en el backend.
