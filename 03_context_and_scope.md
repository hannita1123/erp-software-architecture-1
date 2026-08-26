# Contexto y Alcance del Sistema

## Contexto de negocio
El sistema ERP interactúa con dos tipos de actores principales: los
usuarios internos de la empresa (como el Administrador de Compras, quien
registra productos y proveedores) y sistemas externos, como el Sistema
Contable Externo, al cual el ERP envía la información de facturas y
asientos contables generados por sus operaciones.

A continuación se muestra el diagrama de contexto (C1) del sistema:

![Diagrama de Contexto](docs/images/c1_context.png)

## Explicación
- El **Administrador de Compras** usa el ERP para registrar productos
  y proveedores.
- El **Sistema ERP** centraliza los procesos de negocio de la empresa.
- El ERP envía información de facturas y asientos contables al
  **Sistema Contable Externo**, manteniendo la contabilidad actualizada
  sin duplicar el registro manual de esos datos.
