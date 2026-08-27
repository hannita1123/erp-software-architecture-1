# Decisiones de Arquitectura

## Decisión 1: Arquitectura monolítica vs. microservicios
- **Contexto:** el equipo es pequeño y el proyecto está en una etapa
  inicial.
- **Decisión:** se optó por una arquitectura monolítica en lugar de
  microservicios.
- **Justificación:** un monolito es más simple de desarrollar, probar
  y desplegar en las primeras etapas del proyecto, reduciendo la
  complejidad operativa. La separación en capas (SPA, API, BD) permite
  una futura migración a microservicios si el proyecto crece.

## Decisión 2: PostgreSQL como base de datos
- **Contexto:** se necesita una base de datos robusta y relacional
  para manejar entidades con relaciones claras (Producto, Proveedor,
  Orden de Compra).
- **Decisión:** se eligió PostgreSQL.
- **Justificación:** es un motor de base de datos relacional maduro,
  gratuito, con buen soporte de transacciones y amplia compatibilidad
  con Java/Spring Boot.

## Decisión 3: SPA con React para el frontend
- **Contexto:** se requiere una interfaz de usuario moderna y fluida
  para los usuarios del ERP.
- **Decisión:** se eligió construir una Single-Page Application con
  React.
- **Justificación:** React permite construir interfaces interactivas
  y reutilizar componentes, mejorando la experiencia de usuario y
  la velocidad de desarrollo del frontend.
