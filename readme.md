# FWS (Functional Web Scripting Language) #

FWS es un proyecto de lenguaje de programación diseñado para el desarrollo web, inspirado en la sintaxis y funcionalidad de lenguajes maduros como JavaScript. Su objetivo es ofrecer un rendimiento mejorado y un enfoque en la programación funcional, permitiendo a los desarrolladores construir aplicaciones web de manera eficiente y efectiva.

## Pilares y Conceptos Principales del Lenguaje FWS ##

FWS utiliza paradigmas de programación funcional, que se basan en el uso de funciones como unidades fundamentales de construcción de software. Mediante el uso de este paradigma, FWS toma inspiración directa de la **matemática y el cálculo lambda**, buscando escribir programas más declarativos, expresivos y fáciles de razonar. Al eliminar o controlar los efectos colaterales, el uso de la programación funcional permite construir software más robusto, predecible y fácil de testear.

### Los Principales Motivos ###

- Facilidad en la **razonabilidad** y la comprensión del código.
- Fomentar la **modularidad**, permitiendo crear software a partir de funciones pequeñas y reutilizables.
- Mejorar la **concurrencia y paralelización**, ya que se evitan problemas de estado compartido.
- Reducir errores relacionados con el cambio de estado o la mutación de datos.

### Principios centrales ###

Basado en el paradigma de programación funcional, el lenguaje de programación FWS se apoya en varios pilares conceptuales que lo distinguen claramente de otros lenguajes similares, como los basados en la programación orientada a objetos o la imperativa. Estos principios incluyen la inmutabilidad, el uso de funciones puras, la transparencia referencial, el currying, la composición de funciones, y el uso intensivo de funciones de orden superior.

Comprender estos pilares y conceptos es clave la correcta implementación de un proyecto basado en FWS y para aplicar la programación funcional de manera efectiva.

A continuación se listan los principales **pilares** y **conceptos clave** del lenguaje FWS tomados del paradigma de programación funcional:

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
