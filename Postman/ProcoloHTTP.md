# HTTP
HTTP (Hypertext Transfer Protocol) es un protocolo de comunicación utilizado para transferir información en la web. Funciona como la base de la comunicación de datos en la World Wide Web (WWW).

## Características principales
- **Cliente-Servidor**: HTTP sigue un modelo cliente-servidor donde el cliente realiza solicitudes y el servidor responde con los recursos solicitados.
- **Sin estado**: Cada solicitud HTTP es independiente y no guarda información de solicitudes anteriores.
- **Métodos HTTP**: Los métodos más comunes son GET, POST, PUT, DELETE, HEAD, OPTIONS, PATCH.
- **Códigos de estado**: HTTP utiliza códigos de estado para indicar el resultado de una solicitud. Ejemplos incluyen 200 (OK), 404 (Not Found), 500 (Internal Server Error).

## Estructura de una solicitud HTTP
1. **Línea de solicitud**: Incluye el método HTTP, la URL y la versión del protocolo.
2. **Encabezados**: Proporcionan información adicional sobre la solicitud.
3. **Cuerpo**: Contiene los datos que se envían al servidor (opcional).

## Estructura de una respuesta HTTP
1. **Línea de estado**: Incluye la versión del protocolo, el código de estado y un mensaje descriptivo.
2. **Encabezados**: Proporcionan información adicional sobre la respuesta.
3. **Cuerpo**: Contiene los datos solicitados (opcional).

HTTP es fundamental para la comunicación en la web y es utilizado por navegadores, servidores web y muchas aplicaciones para intercambiar datos.


## Idempotencia
La idempotencia es una propiedad de ciertos métodos HTTP que indica que una solicitud idéntica puede ser realizada una o varias veces con el mismo efecto, sin cambiar el estado del servidor. En otras palabras, realizar la misma operación múltiples veces no tendrá efectos adicionales después de la primera ejecución.

Los métodos HTTP idempotentes son:
- **GET**
- **PUT**
- **DELETE**
- **HEAD**
- **OPTIONS**

## Métodos HTTP más usados
A continuación se describen los métodos HTTP más utilizados:

- **GET**: Solicita un recurso del servidor. No debe tener efectos secundarios y puede ser almacenado en caché.
- **POST**: Envía datos al servidor para crear un nuevo recurso. No es idempotente y no debe ser almacenado en caché.
- **PUT**: Envía datos al servidor para actualizar un recurso existente. Es idempotente.
- **DELETE**: Solicita la eliminación de un recurso en el servidor. Es idempotente.
- **HEAD**: Solicita los encabezados de una respuesta, sin el cuerpo. Útil para comprobar si un recurso existe.
- **OPTIONS**: Describe las opciones de comunicación para el recurso de destino. Es idempotente.
- **PATCH**: Aplica modificaciones parciales a un recurso. No es necesariamente idempotente.


## Tipos de códigos de respuesta HTTP
Los códigos de estado HTTP se dividen en cinco clases, cada una representada por el primer dígito del código de estado:

1. **1xx (Informativos)**: Indican que la solicitud fue recibida y el proceso continúa.
    - 100 Continue
    - 101 Switching Protocols
    - 102 Processing

2. **2xx (Éxito)**: Indican que la solicitud fue recibida, entendida y procesada correctamente.
    - 200 OK
    - 201 Created
    - 202 Accepted
    - 204 No Content

3. **3xx (Redirección)**: Indican que se deben tomar acciones adicionales para completar la solicitud.
    - 301 Moved Permanently
    - 302 Found
    - 304 Not Modified

4. **4xx (Errores del cliente)**: Indican que la solicitud contiene sintaxis incorrecta o no puede ser procesada.
    - 400 Bad Request
    - 401 Unauthorized
    - 403 Forbidden
    - 404 Not Found

5. **5xx (Errores del servidor)**: Indican que el servidor falló al completar una solicitud válida.
    - 500 Internal Server Error
    - 501 Not Implemented
    - 502 Bad Gateway
    - 503 Service Unavailable