# Creacion de APIs

Meta: Crear un conjunto de APIs que expongan distintas fórmulas a los usuarios a través de HTTP endpoints.

- [Exponer las formulas en HTTP endpoints](https://github.com/cs1000-utec/laboratorio5-template) para calcular el `volumen` y `surface area` de todas las figuras geometricas en la imagen `geometry.jpg`.

Requisitos:

- La estructura de las urls deberan de ser:

`/figurageometrica/volumenosurfacearea/parametro1/parametro2/etc...`

Donde

- `figurageometrica`: se refiere a la figura geometrica, e.g. cubo, esfera, etc...

- `volumenosurfacearea`: se refiere a si calculara la formula de `volumen` o `surfacearea`

- `/parametro1/parametro2/etc...`: se refiere a la lista de parametros necesarios para realizar el calculo del resultado

Ejemplo:

- `/cube/volumen/5`: Donde 5 es el valor de `s`

## Presentacion (3 mins)

Mostrar el funcionamiento de todas las APIs e incluir un README.md en el cual se detalle las APIs disponibles, los parametros que deben pasarse en cada uno de ellos y la manera en que su proyecto puede ejecutarse localmente.

## Información adicional para el README

Incluir en el README.md una sección llamada "Especificación del API" en el cual se detalle **para cada API**:

- URL.
- Parametros que recibe la URL y que valor representa cada uno de ellos.
- Salida que devolverá el programa.
- Ejemplo de una invocación a dicha API (url y salida).

Ejemplo:

```
# Especificación del API

## URL
/cube/volumen/:lado

## Parametros
- lado: Lado del cubo

## Salida
Volumen del cubo

## Ejemplo

- URL: localhost:9000/cube/volumen/3
- Salida: 27 (o screenshot de la salida en caso existan gráficos)

...
...
...
```