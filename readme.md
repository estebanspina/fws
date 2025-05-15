# FWS (Functional Web Scripting Language) #

FWS es un proyecto de lenguaje de programación diseñado para el desarrollo web, inspirado en la sintaxis y funcionalidad de lenguajes maduros como JavaScript. Su objetivo es ofrecer un rendimiento mejorado y un enfoque en la programación funcional, permitiendo a los desarrolladores construir aplicaciones web de manera eficiente y efectiva.

## Pilares y Conceptos Principales del Lenguaje FWS ##

### Pilares de FWS ###

1. **Funciones puras:**
   - No tienen efectos secundarios.
   - Devuelven siempre el mismo resultado para los mismos argumentos.
   - No modifican datos externos ni cambian el estado global.

2. **Inmutabilidad:**
   - Los datos no cambian una vez creados.
   - Se crean nuevas versiones de las estructuras de datos en lugar de modificarlas.
   - Facilita el razonamiento y evita errores por estado compartido.

3. **Funciones como ciudadanos de primera clase:**
   - Las funciones pueden asignarse a variables.
   - Se pueden pasar como argumentos y devolver como resultados.
   - Permite el uso de funciones de orden superior.

4. **Transparencia referencial:**
   - Una expresión puede ser reemplazada por su resultado sin cambiar el comportamiento del programa.
   - Mejora la capacidad de razonamiento y permite optimizaciones como memoización.

5. **Evaluación perezosa (Lazy Evaluation):**
   - Las expresiones no se evalúan hasta que es necesario.
   - Permite trabajar con estructuras infinitas y optimizar el rendimiento.
   - (Dependiendo del lenguaje).

6. **Composición de funciones:**
   - Se crean programas complejos combinando funciones simples.
   - Fomenta la reutilización y la modularidad.

### Conceptos Clave ###

| Concepto                      | Descripción breve                                                  |
|-------------------------------|--------------------------------------------------------------------|
| **Funciones puras**            | Sin efectos colaterales, solo entrada → salida.                    |
| **Inmutabilidad**              | Datos no se modifican, se crean nuevas versiones.                  |
| **Funciones de orden superior**| Aceptan y devuelven funciones.                                     |
| **Transparencia referencial**  | Se puede sustituir expresión por su resultado sin problemas.       |
| **Currying**                   | Convierte funciones de varios argumentos en una secuencia de funciones de un solo argumento. |
| **Composición de funciones**   | Combinación de funciones para crear nuevas funciones.              |
| **Recursión**                  | Sustituye bucles; se favorece sobre estructuras imperativas.       |
| **Mónadas (avanzado)**          | Manejan efectos secundarios de manera controlada (como IO, errores). |

## Diagrama conceptual - Programación Funcional ##
Este diagrama muestra cómo todos los pilares se interrelacionan y derivan en prácticas y conceptos avanzados.


                                 +-----------------------------+
                                 |    Programación Funcional    |
                                 +-----------------------------+
                                              |
    ----------------------------------------------------------------------------------
    |                     |                     |                     |             |
+----------------+  +----------------+  +----------------+  +----------------+  +----------------+
| Funciones Puras |  | Inmutabilidad  |  | Funciones como |  | Transparencia  |  | Evaluación     |
|                 |  |                |  | ciudadanos de  |  | Referencial    |  | Perezosa       |
| Entrada -> Salida | | No modifica    |  | primera clase  |  | (Equivalencia  |  | (Lazy Eval)    |
| Sin efectos    |  | datos originales | | Pueden ser     |  | de expresión y |  | Evalúa bajo    |
| secundarios    |  | Crea nuevas     |  | argumentos,    |  | resultado)     |  | demanda        |
+----------------+  | estructuras    |  | retornos       |  +----------------+  +----------------+
                     +----------------+  +----------------+                                   
                                              |
                                              v
                                  +--------------------------+
                                  |  Funciones de orden      |
                                  |  superior y composición  |
                                  +--------------------------+
                                              |
    ---------------------------------------------------------------------------------
    |                             |                           |                    |
+-----------+          +----------------+           +----------------+   +----------------+
| Currying  |          | Composición de |           | Recursión       |   | Mónadas        |
|           |          | funciones       |           | (en vez de      |   | (Efectos      |
| Convierte |          | Construir       |           | bucles)         |   | controlados)  |
| funciones |          | complejidad     |           +----------------+   +----------------+
| multiar.  |          | desde lo simple |
+-----------+          +----------------+
