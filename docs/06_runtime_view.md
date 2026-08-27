# Vista de Tiempo de Ejecución (Runtime)

## Escenario: Registrar un Producto

Este escenario describe cómo interactúan los componentes del sistema
cuando el Administrador de Compras registra un nuevo producto.

![Diagrama de Secuencia](c3_sequence.png)

## Explicación del flujo

1. El **Administrador** llena el formulario de nuevo producto en la
   **SPA** y lo envía.
2. La **SPA** hace una petición `POST /api/productos` a la **API**,
   enviando los datos del producto.
3. La **API** valida los datos recibidos (por ejemplo, que el nombre
   no esté vacío).
4. Si los datos son válidos, la **API** ejecuta un `INSERT` en la
   **Base de Datos** para guardar el nuevo producto.
5. La **Base de Datos** confirma la creación y devuelve el producto
   con su ID generado.
6. La **API** responde a la SPA con un código `201 Created` y los
   datos del producto creado.
7. La **SPA** muestra un mensaje de éxito al Administrador y actualiza
   la lista de productos en pantalla.
