# Riesgos Técnicos y Deuda Técnica

## Riesgos identificados

### Riesgo 1: Escalabilidad del monolito
- **Descripción:** al concentrar toda la lógica de negocio en una sola
  API monolítica, un aumento significativo de usuarios podría afectar
  el rendimiento de todo el sistema a la vez.
- **Mitigación:** diseñar la API con módulos internos bien separados
  (por ejemplo, compras, facturación, empleados), de modo que sea más
  sencillo extraerlos como microservicios independientes en el futuro
  si es necesario.

### Riesgo 2: Dependencia de un único proveedor de base de datos
- **Descripción:** toda la información del ERP depende de una sola
  instancia de PostgreSQL; si esta falla, el sistema completo queda
  no disponible.
- **Mitigación:** implementar respaldos (backups) periódicos y, a
  futuro, considerar una configuración de alta disponibilidad
  (réplicas de base de datos).

### Riesgo 3: Validaciones duplicadas entre frontend y backend
- **Descripción:** al validar datos tanto en la SPA como en la API,
  existe el riesgo de que ambas validaciones queden desincronizadas
  con el tiempo.
- **Mitigación:** documentar claramente las reglas de negocio y
  mantener la API como la única fuente de verdad para las
  validaciones críticas.

## Deuda técnica conocida
- Actualmente no se ha definido un mecanismo de autenticación y
  autorización de usuarios, lo cual deberá implementarse antes de
  llevar el sistema a producción.
