# Tipos de datos
Un dato es menos que información, y se utilizan para clasificar los datos con los que cuentan los sistemas operativos, mientras que un conjunto de datos si representa información.

## Clasificación de los datos

### Numericos
    - Enteros
    - Reales
### Texto
    - Caracter (Datos alfanumericos ASCII)
    - Cadenas de texto
### Lógicos
    - Boolean (Falso y verdadero)

## Comunicación entre API's

API es el puente que une las aplicaciones y JSON es el lenguaje que usan para comunicarse comunmente.

¿Cómo se envía la información?
Comunmente mediante el protocolo HTTP

### JSON
Javascript Object Notation. Es un formato ligero de intercambio de datos, es fácil de leer y escribir para seres humanos y simple de interpretar y generar para los equipos de computo.
Es un formato de texto independiente del lenguaje de programación, ideal para el intercambio de datos.

#### Ejemplo formato json:
```json
Persona = {
    "Id":"1",
    "Nombre":"Jhon",
    "Apellido":"Doe",
    "Edad":64,
    "Tel":null,
    "Check":true,
    "SO":["Windows","Ubuntu","Android"]
}
```

