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

## Diagrama conceptual ##
Este diagrama muestra cómo todos los pilares se interrelacionan y derivan en prácticas y conceptos avanzados.

[![](https://mermaid.ink/img/pako:eNpdUs1uGjEQfhXLZ4J2F-j-HCq1kKRJWglFOdWbw3RtwO3asxqvqwLiqfIIebHY0KCwPnnm-xn7s_e8Qal4xdcE3YY9LWqqLQvri1gShqaBRr--WHbjbaPRQvscGWcWu7r6zL6K_6hybOkJ3PMlPhd31vgefulWS5ADdPFB3aBB1mgfWGDRMalYR9ooAta04NRAei2eCKzrgFRwAPaoVuq0bQfMG3H9F1oPcQ5bBtIOHTAk9h12Wxaxi3stjqLbDycLJ0GSyjLnO0Ua6Tzg9sj9JuaeaKvtegDciTmaDp0-5Rh8Vu-mFyNP7HvxqBpPLnIHRg_iR2iGYBxDZsCq3xjdwpWbHmN0tidsQeLJl4_Cm2rJq568GvGQoYFY8n00rXm_UUbVvApbCfSn5rU9BE0H9ieieZcR-vWGVytoXah8J6FXCw3xY5y7IXGpaI7e9rxKi-Jowqs9_xfKtByXs3xWFGk5K5IkD-iWV1mSjWfJJMnSbJpkk-mkOIz47jg3GRf5tCzL_FOSTtIszYvDG3wV2yc?type=png)](https://mermaid.live/edit#pako:eNpdUs1uGjEQfhXLZ4J2F-j-HCq1kKRJWglFOdWbw3RtwO3asxqvqwLiqfIIebHY0KCwPnnm-xn7s_e8Qal4xdcE3YY9LWqqLQvri1gShqaBRr--WHbjbaPRQvscGWcWu7r6zL6K_6hybOkJ3PMlPhd31vgefulWS5ADdPFB3aBB1mgfWGDRMalYR9ooAta04NRAei2eCKzrgFRwAPaoVuq0bQfMG3H9F1oPcQ5bBtIOHTAk9h12Wxaxi3stjqLbDycLJ0GSyjLnO0Ua6Tzg9sj9JuaeaKvtegDciTmaDp0-5Rh8Vu-mFyNP7HvxqBpPLnIHRg_iR2iGYBxDZsCq3xjdwpWbHmN0tidsQeLJl4_Cm2rJq568GvGQoYFY8n00rXm_UUbVvApbCfSn5rU9BE0H9ieieZcR-vWGVytoXah8J6FXCw3xY5y7IXGpaI7e9rxKi-Jowqs9_xfKtByXs3xWFGk5K5IkD-iWV1mSjWfJJMnSbJpkk-mkOIz47jg3GRf5tCzL_FOSTtIszYvDG3wV2yc)
